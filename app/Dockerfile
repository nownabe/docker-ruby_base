FROM nownabe/ruby_base:2.2.2-base
MAINTAINER nownabe <nownabe@gmail.com>

RUN bundle config --global frozen 1

RUN mkdir /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY Gemfile /usr/src/app/
ONBUILD COPY Gemfile.lock /usr/src/app/
ONBUILD RUN bundle install

ONBUILD COPY . /usr/src/app
