# redis-server-docker

## Configure Redis

Create `redis_conf/redis.conf` file with the following content:

```bash
requirepass your_redis_password
```

## Start Redis

```bash
mkdir redisinsight_data
chmod 777 redisinsight_data

docker compose up -d
```

- redis: `localhost:6379`
- redisinsight: `localhost:5540`
  - host: `redis`
  - port: `6379`
  - username: `default`
  - password: `your_redis_password`