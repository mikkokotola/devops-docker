FROM ubuntu:16.04

WORKDIR /usr/app
COPY . .

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN npm install
RUN npm audit fix
EXPOSE 5000

CMD API_URL=http://localhost/api/ npm start
