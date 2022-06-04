FROM redis:7.0.0-alpine AS redis

ADD ./redis.conf /usr/local/etc/redis/redis.conf

HEALTHCHECK --interval=60s --retries=3 --timeout=5s  CMD redis-cli ping

CMD redis-server /usr/local/etc/redis/redis.conf --requirepass ${REDIS_PASSWORD}
