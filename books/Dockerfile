FROM node:18.16.0-slim
USER ${USER}
WORKDIR /usr/src/books
COPY ./books/package*.json ./
COPY ./books ./
RUN apt-get -y update; apt-get -y install curl
RUN npm install --silent
EXPOSE 3000
CMD npm run dev