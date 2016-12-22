# Acquire full infrastructure

This repository describes the whole Acquire application stack using Docker and Docker Compose.

## Usage

Build and spin up both of our containers at the same time:

`docker-compose up --build -d`

The `--build` flag indicates that we want to build our images if necessary using the build section under each of our services in the 
config file. The `-d` parameter tells Docker Compose to run the containers in the background.

## References

* https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/
* http://dapperdeveloper.com/2016/05/18/developing-with-docker-and-webpack/
* http://moduscreate.com/optimizing-react-es6-webpack-production-build/
* http://www.pro-react.com/materials/appendixA/