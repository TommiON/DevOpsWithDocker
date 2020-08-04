FROM ruby:2.6.0
WORKDIR /workdir
COPY . .
RUN apt -y update && apt -y upgrade 
RUN apt -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
EXPOSE 3000
CMD rails s