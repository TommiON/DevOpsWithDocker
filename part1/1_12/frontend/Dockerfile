FROM ubuntu:16.04
WORKDIR /mydir
COPY . .
RUN apt -y update && apt -y upgrade 
RUN apt -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
EXPOSE 5000
ENV API_URL=http://localhost:8000
CMD ["npm", "start"]