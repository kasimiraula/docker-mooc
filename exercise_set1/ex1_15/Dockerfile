FROM ubuntu:16.04
COPY dockerhub-example/clickingapp .
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
RUN npm install -g serve
RUN npm run build
RUN ls
EXPOSE 3000
CMD serve -s -l 3000 build
