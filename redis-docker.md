#Redis Note

#Docker image
https://redis.io/docs/getting-started/.

#How to use
1. Start the docker:
    docker run --name my-redis -p 6379:6379 -d redis
2. Start the shell:
    docker exec -it my-redis sh
3. Alternatively, download redis-cli and run it.
    redis-cli
