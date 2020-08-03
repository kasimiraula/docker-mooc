FROM ruby:2.6.0
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
COPY rails-example-project ./
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD rails s

