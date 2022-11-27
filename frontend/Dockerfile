FROM node:19.0
WORKDIR /usr/src/app
COPY package*.json ./
EXPOSE 5173
COPY . .
RUN apt-get update && npm install
CMD npm run dev
