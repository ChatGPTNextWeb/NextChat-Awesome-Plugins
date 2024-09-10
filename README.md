# NextChat-Awesome-Plugins

This project stores [Plugins](https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web/issues/5353) for [ChatGPT-Next-Web](https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web)


## Design
1. config plugin, like GPTs  action (openapi schema + authentication).
2. wrap API to `javascript` function,  then using [function-calling](https://platform.openai.com/docs/guides/function-calling)`
![image](https://github.com/user-attachments/assets/b7cfc13b-e9e8-46c0-bee5-4fa71e51bfff)


## Plugins

| Name | Authentication | Description |
| ---- | --- | ----------------------------- |
| [Dalle3](./plugins/dalle) | bearer | openai's dall-e image generator|
| [FluxPro](./plugins/flux) | custom | The pro version of FLUX.1, served in partnership with BFL |
| [WolframAlpha](./plugins/wolframalpha) | custom | A wrapper around Wolfram Alpha |
| [ArxivSearch](./plugins/arxivsearch) | - | Run Arxiv search and get the article information |
| [DuckDuckGoLiteSearch](./plugins/duckduckgolite) | - | a search engine |
| [gapier](./plugins/gapier) | bearer | A free exclusive GPTs Actions API provided by gapier.com |
| [Webpilot](./plugins/webpilot) | custom | from: https://www.webpilot.ai |
| [FastGPT](./plugins/fastgpt) | bearer | |
| [NPM Registry Search API](./plugins/npmsearch) | - | Search for packages in the NPM registry |
| [CodeInterpreter](./plugins/codeinterpreterapi) | - | from: [leezhuuuuu/Code-Interpreter-Api](https://github.com/leezhuuuuu/Code-Interpreter-Api) |
| [Chat PDF](./plugins/chatpdf) | - | from: [PDF AI Reader Chat (4.1 ★)](https://chatgpt.com/g/g-oMM2c1bD3) |

