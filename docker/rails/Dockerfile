FROM ruby:2.6.3

RUN apt-get update -qq && apt-get install -y build-essential nodejs
RUN mkdir -p /app

WORKDIR /app

ADD Gemfile /app/Gemfile
ADD Gemfile.lock /app/Gemfile.lock

RUN bundle install
ADD . /app
