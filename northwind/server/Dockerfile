FROM node:latest

LABEL name="northwindapp"
LABEL maintainer="b@nus.edu.sg"

ENV DB_HOST=mydb
ENV DB_PORT=3306
ENV APP_PORT=3000
ENV APP_DIR=/app 

WORKDIR ${APP_DIR}

ADD . .

RUN npm install
EXPOSE ${APP_PORT}
ENTRYPOINT [ "node", "main.js" ]