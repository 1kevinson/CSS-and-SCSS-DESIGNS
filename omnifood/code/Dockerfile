FROM node:15.14.0-alpine3.10

RUN echo "alias ll='ls -la'" >> ~/.bashrc 

WORKDIR /app

COPY package.json .

RUN npm install

VOLUME ["/app/node_modules"]

COPY . .

EXPOSE 8080

CMD ["npm","start"]

LABEL version="1.0" 