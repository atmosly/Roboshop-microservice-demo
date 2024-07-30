FROM node:14

ENV INSTANA_AUTO_PROFILE true

EXPOSE 8080

WORKDIR /opt/server

COPY atmosly-user/package.json /opt/server/

RUN npm install

COPY atmosly-user/server.js /opt/server/

CMD ["node", "server.js"]

