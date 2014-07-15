FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y curl

ENTRYPOINT ["sh", "-c", "curl https://gender-api.com/get?name=$0"]

CMD ["thomas"]
