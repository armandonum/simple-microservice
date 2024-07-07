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

cree su aplicación .NET Core en una imagen de Docker:
```bash
docker build -t microservice1 .
```
ejecute su contenedor Docker
```bash 
docker run -it --rm -p 3000:8080 --name Services microservice1
```

