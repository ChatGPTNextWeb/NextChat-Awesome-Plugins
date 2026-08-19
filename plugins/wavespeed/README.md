# WaveSpeed

> Generate images and videos with [WaveSpeed AI](https://wavespeed.ai) — ByteDance Seedream / Seedance, FLUX, and the rest of the wavespeed.ai model catalog, served on a fast async prediction API.

> Get an API key from the [WaveSpeed dashboard](https://wavespeed.ai/dashboard/apikeys). API reference: [wavespeed.ai/docs](https://wavespeed.ai/docs)

## Schema
[openapi.json](./openapi.json)

## Servers

`https://api.wavespeed.ai`

## Operations

1. `WaveSpeedSubmit` — `POST /api/v3/{model_id}` submits a generation task with `{"prompt": "..."}` and returns a prediction id. Default image model: `bytedance/seedream-v5.0-pro`. Any model id from [wavespeed.ai/models](https://wavespeed.ai/models) works, e.g. `bytedance/seedance-v1-pro-t2v-720p` for text-to-video.
2. `WaveSpeedGetResult` — `GET /api/v3/predictions/{id}/result` polls the task. The model should call it again while `data.status` is `created`/`processing`, and when it is `completed`, show `data.outputs[0]` (the generated image/video URL) to the user.

All responses use the envelope `{code, message, data: {id, status, outputs, error}}`.

## Authentication

```
type: bearer
location: header
```

Paste your WaveSpeed API key (from [wavespeed.ai/dashboard/apikeys](https://wavespeed.ai/dashboard/apikeys)) as the token.
