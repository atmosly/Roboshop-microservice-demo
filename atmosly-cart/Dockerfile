FROM node:14

ENV INSTANA_AUTO_PROFILE true

EXPOSE 8080

WORKDIR /opt/server

COPY atmosly-cart/package.json /opt/server/

RUN npm install

COPY atmosly-cart/server.js /opt/server/

CMD ["node", "server.js"]

