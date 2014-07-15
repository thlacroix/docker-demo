FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y curl

ENTRYPOINT ["sh", "-c", "curl -s http://api.genderize.io?name=$0"]

CMD ["thomas"]
