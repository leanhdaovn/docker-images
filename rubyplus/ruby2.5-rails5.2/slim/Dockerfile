FROM ruby:2.5.3-slim

RUN apt-get update -qq && apt-get install -y \
  build-essential \
  patch \
  ruby-dev \
  zlib1g-dev \
  liblzma-dev \
  libxml2-dev \
  libpq-dev

WORKDIR /app
COPY Gemfile /app

RUN bundle install

CMD ["bash"]
