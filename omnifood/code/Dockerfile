FROM node:15.14.0-alpine3.10

RUN echo "alias ll='ls -la'" >> ~/.bashrc 

WORKDIR /app

COPY package.json .

RUN npm install --silent

VOLUME ["/app/node_modules"]

COPY . .

CMD ["npm","start"]

LABEL version="1.0" 