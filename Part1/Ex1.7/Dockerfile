FROM ubuntu:16.04

WORKDIR /usr/app
COPY curler.sh .
RUN chmod +x ./curler.sh
RUN apt-get update && apt-get install -y curl

CMD ["./curler.sh"]