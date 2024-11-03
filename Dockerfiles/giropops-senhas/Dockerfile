FROM ubuntu:20.04
RUN apt-get update && apt-get install pip -y && apt-get clean
EXPOSE 5000
WORKDIR /app/giropops-senhas
ADD . .
RUN pip3 install --no-cache-dir -r requirements.txt
ENV REDIS_HOST="redis"
ENTRYPOINT ["python3"]
CMD ["-m","flask","run","--host=0.0.0.0"]
