## REDIS CONTAINER

# FOR shell inside this container
> docker exec -it redis_container /bin/sh

## Other commands
```bash
> redis-benchmark -n 1000000 incr foo
> redis-cli object freq foo
```

## PORTS
```
1. redis : 5050
2. rabbitmq : 5051
```