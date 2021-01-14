# SCA-Cloud-School-Application

To successfully build and run this application, you should have Docker installed.

## Deployment Instructions

- Clone repo
```sh
git clone https://github.com/Goodiec/SCA-Cloud-School-Application.git
```

- Change directory
```sh
cd SCA-Cloud-School-Application
```

- Build the Docker image
```sh
docker build -t web-app .
```

- Run the Docker image
```sh
docker run -p 8888:8080 -d web-app 
```
Going to http://localhost:8888 should display the webpage

- Test the app to get container ID and the port that was mapped by Docker
```sh
docker ps
```

- Print app output
```sh
docker logs <container ID>
```

- Call the application
```sh
curl -i localhost:<the port that Docker mapped, e.g - 8888>
```

[Docker Hub Repository](https://hub.docker.com/u/goodiec)
