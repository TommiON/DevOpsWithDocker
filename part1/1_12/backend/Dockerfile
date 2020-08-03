FROM ubuntu:16.04
WORKDIR /mydir
COPY . .
RUN apt -y update && apt -y upgrade 
RUN apt -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
EXPOSE 8000
ENV FRONT_URL=http://localhost:5000
CMD ["npm", "start"]