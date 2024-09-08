# AI Playground

Quickly get AI up and running locally.

## What it does

This docker compose file will run an instance of [Ollama](https://ollama.com/) and an instance of the 
[Open WebUI](https://docs.openwebui.com/), so you can easily talk to the model of your choice.

Upon running, two local directories will be created in order not to lose data between runs (you don't
want to download the models every time you run this docker compose):

* `ollama`
* `open-webui`

Open WebUI's default authentication is disabled.

## Requirements

Docker! :rocket:
g
## Startup

```
docker compose up
```

## Download a model

From the command line, run
```
curl http://localhost:11434/api/pull -d '{"name":"llama3.1"}'
```

## Usage

Open Firefox and go to `http://localhost:3000`