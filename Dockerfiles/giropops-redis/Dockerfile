FROM ubuntu:20.04
RUN apt-get update && apt-get install redis -y && apt-get clean
EXPOSE 6379
ENTRYPOINT ["redis-server"]
CMD ["--protected-mode", "no"]
