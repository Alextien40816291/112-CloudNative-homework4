FROM node:latest

WORKDIR /backend

COPY package*.json .

RUN npm install

COPY . .

COPY .env.sample .env

RUN npm run build

EXPOSE 8888

CMD [ "npm", "run", "dev" ]