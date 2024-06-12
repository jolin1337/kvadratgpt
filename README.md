# kvadratgpt

This repository is a simple combination of Ollama, Open WebUI and Automatic1111-Stable Diffusion models that works together in a docker compose file, ready to be deployed in a on prem environment.

## Preparations

You would need a computer with quite some Memory resources 16GB+, it is setup to work on only the CPU but GPU is possible to enable by providing the nvidia/amd runtime in the compose file. You would also need [docker](https://www.docker.com/) and [docker-compose](https://docs.docker.com/compose/) installed on the computer.

## Installation

1. Clone this repo: `git clone https://github.com/jolin1337/kvadratgpt.git && cd kvadratgpt`
2. If you want GPU support go into `./docker-compose.yaml` and ad `runtime: nvidia` to the services you'd like to have GPU support for, otherwise you are already setup to start the application
3. Now just run: `docker compose up -d automatic1111 open-webui ollama`


## Features

Current supported features are constantly updated by the creators of these amazin products, although this is a list of some major ones:
 - ChatGPT like Interface ([open-webui](https://docs.openwebui.com/features))
 - ChatGPT like Custom Agents ([open-webui](https://docs.openwebui.com/features))
 - Information retireval through RAG ([open-webui](https://docs.openwebui.com/features))
 - Image generation based on a prompt ([automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Features))
 - Community driven GPT Model and prompt support ([open-webui community](https://openwebui.com/))
 - All is local and no information is shared with anyone but the users of the local instance
 - Integration support with other tools such as (but not limited to) developer IDE:s [Continue](https://docs.continue.dev/intro) and [ollama](https://ollama.com/)
