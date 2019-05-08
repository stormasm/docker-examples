
This
[description by markheath](https://markheath.net/post/exploring-redis-with-docker)
explains a simple way to talk to redis

```
docker run -d -p 6379:6379 --name redis1 redis
docker exec -it redis1 sh
redis-cli
```
