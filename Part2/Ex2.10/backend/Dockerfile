FROM ubuntu:16.04

WORKDIR /usr/app
COPY . .

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN npm install
RUN npm audit fix
EXPOSE 8000

CMD FRONT_URL=http://frontend:5000 npm start
