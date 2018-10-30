FROM redis:3.2

COPY redis.conf /etc/redis/redis.conf

# set timezome
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN chmod 777 /etc/redis/redis.conf

CMD ["redis-server", "/etc/redis/redis.conf"]
