FROM ubuntu
WORKDIR /workdir
ADD frontend-example-docker-master ./
RUN apt-get update && apt-get install -y curl && curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
CMD API_URL=http://localhost:8000 npm start