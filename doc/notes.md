
#### In these notes

#### How to install docker

```
snap install docker
```

#### How to uninstall docker

```
snap remove docker
```

#### How to check that docker was removed

```
snap list
```

#### Pull your image

[Pull an image from a registry](https://docs.docker.com/engine/reference/commandline/pull/)

```
docker pull <image name>
```

[Pull the nginx image](https://hub.docker.com/_/nginx/)

```
docker pull nginx
```

Delete an image from the local image store

```
docker rmi <image name>
```

*santafe* is an example tag name.   
docker maps the port *8080* port inside the container to the port *3000* on your machine.

Go to the directory that has your *Dockerfile* and run the following commands

#### Build your image

```
docker build -t santafe .
```

#### List your images

```
docker images
```

#### Run your image

```
docker run -p 3000:8080 -d santafe
```

* -d run the container in detached mode leaving the container running in the background
* -p redirects a public port to a private port

#### Get your container ID

```
docker ps
```

#### Logs

```
docker logs <container id>
```

#### Go inside your container

```
docker exec -it <container id> /bin/bash
```

### References

https://nodejs.org/en/docs/guides/nodejs-docker-webapp/
