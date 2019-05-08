
This
[description by markheath](https://markheath.net/post/exploring-redis-with-docker)
explains a simple way to talk to redis

```
docker run -d -p 6379:6379 --name redis100 redis
```

At this time you can just connect to redis via

```
redisc
```

or you can run this next command as well...

```
docker exec -it redis100 sh
redis-cli
```
