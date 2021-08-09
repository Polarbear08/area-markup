FROM node:14
LABEL maintainer mas

WORKDIR /opt/server

COPY ./package.json /opt/server/package.json

RUN npm install

COPY ./server/server.js /opt/server/server.js
COPY ./docs /opt/docs

CMD [ "node", "/opt/server/server.js" ]