FROM node:18.16.0-slim
USER ${USER}
WORKDIR /usr/src/authors
COPY ./authors/package*.json ./
COPY ./authors ./
RUN apt-get -y update; apt-get -y install curl
RUN npm install --silent
EXPOSE 3001
CMD npm run dev