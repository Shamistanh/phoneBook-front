FROM node:alpine

WORKDIR /usr/src/app


COPY package*.json ./

RUN npm install

ARG BACKEND_URL

ENV BACKEND_URL $BACKEND_URL

COPY . .

EXPOSE 80

CMD ["node", "index.js"]