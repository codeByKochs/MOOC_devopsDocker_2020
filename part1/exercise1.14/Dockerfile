FROM ruby:2.6.0

WORKDIR /usr/app

RUN apt-get update
RUN apt-get install nodejs -y
RUN git clone https://github.com/docker-hy/rails-example-project.git .
WORKDIR /usr/app/rails-example-project
RUN bundle install
RUN rails db:migrate

EXPOSE 3000

CMD ["rails", "s", "-p", "3000", "-b", "'0.0.0.0'"]

#TODO finish this