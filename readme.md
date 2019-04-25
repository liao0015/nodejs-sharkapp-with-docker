# Docker with nodejs (a love story)

A simple nodejs/express app that is managed by docker (demo by DigitalOcean)

## RUN Without docker

```bash
# run application
node app.js
# check the website
localhost:8080
```

## RUN With docker :)

The key is inside 'Dockerfile'

```bash
# build docker image
docker build -t docker-chat-demo .
# run container from image
docker run --name docker-chat-demo -p 80:8080 -d docker-chat-demo
# check the website at
192.168.99.100
```

- [basic app from digitalocean](https://www.digitalocean.com/community/tutorials/how-to-build-a-node-js-application-with-docker)
- [Lessons from Building a Node App in Docker](https://jdlm.info/articles/2016/03/06/lessons-building-node-app-docker.html)
- [Docker and Node.js Best Practices](https://github.com/nodejs/docker-node/blob/master/docs/BestPractices.md)

- [Dockerizing a Node.js web app](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)

## updates

### let's add `nodemon` into Dockerfile