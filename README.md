# github-webhooks-elasticsearch

## Requirements
- [Docker and docker-compose](https://docs.docker.com/get-docker/)
- [Ngrok](https://dashboard.ngrok.com/get-started)


#### Start

1. Docker - `docker-compose up -d`
2. ngrok for local machine `./ngrok http 5400` <- Configurated port for logstash

#### Stop

`docker-compose down`


## Useful links
- `https://developer.github.com/webhooks/`
- `https://developer.github.com/webhooks/configuring/`
