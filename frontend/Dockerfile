FROM node:alpine

WORKDIR /usr/src/app


COPY package*.json ./

RUN npm install

ARG BACKEND_URL

ENV BACKEND_URL $BACKEND_URL

COPY . .

EXPOSE 5000

# the command that starts our app
CMD ["node", "index.js"]