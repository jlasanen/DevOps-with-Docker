FROM ubuntu:16.04

RUN echo "calling apt-get"
RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN apt-get install -y git
RUN git clone  https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /frontend-example-docker
RUN npm install
CMD npm start

