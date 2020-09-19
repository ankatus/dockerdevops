FROM ubuntu
WORKDIR /workdir
ADD backend-example-docker-master ./
RUN apt-get update && apt-get install -y curl && curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
CMD FRONT_URL=http://127.0.0.1:5000 npm start