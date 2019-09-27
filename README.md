# ui5-ide-docker
UI5 development environment in a docker container.
It uses node.js and the UI5 tooling to serve the app.

## Build docker container
docker build -f Dockerfile_fw -t ui5-ide-docker .

## Run docker container
docker run -d -p 8080:8080 -v $(pwd)/app:/usr/src/app flow1985/ui5-ide-docker

## Jump into container
docker exec -it ${containerid} /bin/bash

## Useful links
* [UI5 tooling](https://github.com/SAP/ui5-tooling)
