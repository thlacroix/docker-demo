FROM node

RUN apt-get update -y
RUN apt-get install -y imagemagick

ADD ./node-express-mongoose-demo /usr/src/app
WORKDIR /usr/src/app

RUN npm install

EXPOSE 3000

CMD ["node", "server.js"]
