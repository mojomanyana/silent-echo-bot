FROM node:6.3.0

MAINTAINER jkelvie

EXPOSE 443 3000

WORKDIR /opt

RUN mkdir silent-echo-bot

WORKDIR /opt/silent-echo-bot

COPY bin/ ./bin/

COPY src/ ./src/

COPY static/ ./static/

COPY *.json ./

RUN npm install

RUN npm run tsc

CMD npm start

