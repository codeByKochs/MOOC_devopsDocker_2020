FROM ubuntu:16.04

WORKDIR /
COPY ./backend-example-docker .

RUN apt-get update && apt-get install curl -y && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt install -y nodejs && \
    apt-get purge -y --auto-remove curl && \ 
    rm -rf /var/lib/apt/lists/* 

EXPOSE 8000

WORKDIR /app
CMD npm start