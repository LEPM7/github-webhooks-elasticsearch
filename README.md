# github-webhooks-elasticsearch

## Requirements
- [Docker and docker-compose](https://docs.docker.com/get-docker/)
- [Ngrok](https://dashboard.ngrok.com/get-started)


### Configuration
1. Run grok and grab the forwarding url
![](./docs/run_grok.png)
2. Go to webhooks from your repo and click on create webhook
![](./docs/gotowebhooks.png)
3. Generate a secret token and paste the url from grok like this
![](./docs/config_grok_url.png)
4. Install jenkins logstash plugin. ![](https://miro.medium.com/max/700/1*rcNkgzxcuPE-K7fG2fhYow.png)
5. Configure plugin ![](https://miro.medium.com/max/700/1*GO2ZUnK0b_cPvgG3MWL_cw.png)
6. Create a job in jenkins ![](https://miro.medium.com/max/700/1*xic3nsVbq-yxpreWH_Z0Iw.png)


#### Start

1. Docker - `docker-compose up -d`
2. ngrok for local machine `./ngrok http 5400` <- Configurated port for logstash

#### Stop

`docker-compose down`


## Useful links
- `https://developer.github.com/webhooks/`
- `https://developer.github.com/webhooks/configuring/`
- `https://medium.com/@Raghwendra.sonu/integrate-jenkins-with-github-project-and-feed-the-build-logs-into-elasticsearch-with-logstash-6a50d484bb9d`
