# Anleitung: 

Eine Firma möchte ihre bereits Containerisierte Webanwendung auf AWS ECS bereitstellen.

Hierzu gehe durch folgende Schritte: 
- Forke dieses Repository
- Klone zunächst das repository auf deine lokale Maschine
- Überprüfe mit ```docker compose up```, ob alles funktioniert wie es soll

- Die Frontend und Backend Images müssen in ein privates ECR repository
- Docker compose file so anpassen, dass front und backend aus repo bezogen werden
- ecs-cli herunterladen
- Mit der ecs-cli einen cluster erstellen
- Mit der ecs-cli das compose file benutzen um unsere app in einem cluster zu starten
- Netzwerkeinstellungen vornehmen, dass die App erreichbar ist


A demonstration of Docker to implement a simple 3 tier architecture

* frontend will be able to access the mid-tier
* mid-tier will be able to access the db

In order to run this in docker, simply type ```docker-compose up``` at the command prompt. Docker will then create the [MongoDB](https://www.mongodb.com/) from the stock [mongo](https://hub.docker.com/_/mongo) image. The api uses [nodejs](https://nodejs.org/) with [express](http://expressjs.com/) and is built from a [node:alpine](https://hub.docker.com/_/node) image. The front end uses [ReactJS](https://reactjs.org/) and built from a [node:alpine](https://hub.docker.com/_/node) image.
