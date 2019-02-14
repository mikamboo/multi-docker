# Docker multi containers deploy

[![Build Status](https://travis-ci.org/mikamboo/multi-docker.svg?branch=master)](https://travis-ci.org/mikamboo/multi-docker)

Tutorial revisited from [StephenGrider multi-docker](https://github.com/StephenGrider/multi-docker).

The app to deploy must be abble to calculate and store items of Fibbonacci sequence.

## About this

This is an POC of multi container application to deploy on AWS, GCP ...

## Folders and file

```
├── client
│   └── Dockerfile (Image: mikamboo/tuto-multi-client)
├── nginx
│   └── Dockerfile (Image: mikamboo/tuto-multi-nginx)
├── server
│   └── Dockerfile (Image: mikamboo/tuto-multi-server)
├── worker
│   └── Dockerfile (Image: mikamboo/tuto-multi-worker)
├── Dockerrun.aws.json
├── README.md
```

* Each service has its own Docker file
* The `.travis.yml` CI config is configurer to build and push images to docker hub.
