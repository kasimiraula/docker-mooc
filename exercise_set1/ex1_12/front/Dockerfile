FROM ubuntu:16.04
COPY frontend-example-docker .
RUN pwd
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
EXPOSE 5000
ENV API_URL=http://localhost:8888
CMD npm start
