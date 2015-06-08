FROM nownabe/ruby_base:2.2.1-base
MAINTAINER nownabe <nownabe@gmail.com>

RUN mkdir /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY . /usr/src/app
ONBUILD RUN bundle install

CMD ["bundle", "exec", "rake", "spec"]
