FROM ruby:2.6.0

WORKDIR /usr/app

RUN apt-get update && \
    git clone https://github.com/docker-hy/rails-example-project.git . && \
    bundle install && \
    rails db:migrate && \

CMD ["rails", "s"]

#TODO finish this