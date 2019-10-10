FROM ruby:2.6.0
WORKDIR /app
COPY . .
RUN apt-get update && apt-get install nodejs -yes
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
EXPOSE 3000
ENTRYPOINT ["rails","s"]
