
#### In these notes

*santafe* is an example tag name.   
docker maps the port 8080 port inside the container to the port 3000 on your machine.

#### Build your image

```
docker built -t santafe .
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
