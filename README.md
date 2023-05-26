# GPT Lite Minimal

English | [简体中文](./README.zh-CN.md)

GPT Lite Minimal is a lightweight, fast ChatGPT UI demo application built using Next.js and AntD. It supports both OpenAI and Azure OpenAI accounts.

For a full-featured ChatGPT UI, visit [gptlite](https://github.com/blrchen/gptlite).

[Live Demo](https://gptlite-minimal.vercel.app)
![demo](./docs/images/demo.jpg)

## Prerequisites

You need either an OpenAI account or an Azure OpenAI account.

## Running Locally

1. Install NodeJS 18.
2. Clone the repository.
3. Install dependencies with `npm install`.
4. Set the `OPENAI_API_KEY` environment variable.
5. Start the application using `npm run dev`.
6. Visit `http://localhost:3000` in your browser.

## Run with Docker

1. Clone the repository and navigate to the root directory.
2. Update the `OPENAI_API_KEY` environment variable in the `docker-compose.yml` file.
3. Build the application using `docker-compose build .`
4. Start it by running `docker-compose up -d`.

## One-click Deploy on Vercel

Click the button below to deploy to Vercel:
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fblrchen%2Fgptlite-minimal&project-name=gptlite-minimal&framework=nextjs&repository-name=gptlite-minimal)

## Environment Variables

For OpenAI-specific environments:

| Name                | Description                                                                                                                      | Default Value         |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| OPENAI_API_BASE_URL | Use only if you intend to use a reserved proxy for `api.openai.com`.                                                            | `https://api.openai.com` |
| OPENAI_API_KEY      | Obtain secret key string from the [Open AI API website](https://platform.openai.com/account/api-keys).                              |

For Azure Open AI-specific environments:

| Name                       | Description                                    |
|----------------------------|------------------------------------------------|
| AZURE_OPENAI_API_BASE_URL  | Endpoint (e.g., https://xxx.openai.azure.com). |
| AZURE_OPENAI_API_KEY       | Key                                            |
| AZURE_OPENAI_DEPLOYMENT    | Model deployment name                          |

## Contribution
We welcome PRs of any size.

## Disclaimers
This code is intended solely for demonstration and testing purposes.