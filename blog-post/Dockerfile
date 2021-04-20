FROM node:15.14.0-alpine3.10

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 8080

VOLUME ["/app/node_modules"]

CMD ["npm","start"]

LABEL version="1.0" 