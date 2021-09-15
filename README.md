# Rails 5 Docker Blueprint  
A starting point for building Rails 5 apps in a Docker container using [this link](https://docs.docker.com/samples/rails/) as the baseline.

For initial install run the following commands:
1. To build the docker image and install required depencencies
```bash
docker-compose up
```
2. Initialize the PostGRESQL databases inside the container so rails will work
```bash
docker-compose run web rake db:create
```

On subsequent startups, just run 
```bash
docker-compose up
```
and the app will be availabe on localhost:3000
