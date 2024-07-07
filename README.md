# Simple microservices
This is a simple demo of microservices implemented with Docker.Shows how to build and deploy independent services that work together. 

## previous requisites
- Docker  install 
- Docker Compose 
- .NET SDK (for local development and testing)

##  instalation 
to prepare the development environment

[install docker](https://docs.docker.com/get-docker/) 

[Install .NET SDK](https://dotnet.microsoft.com/download)

## execution

build your .NET Core app in a Docker image:

```bash
docker build -t microservice1 .
```
run your Docker container:

```bash 
docker run -it --rm -p 3000:8080 --name Services microservice1
```

