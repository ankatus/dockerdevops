FROM ruby:2.6.0
WORKDIR /workdir
ADD rails-example-project-master ./
RUN apt-get update
RUN apt-get -y install nodejs
RUN bundle update --bundler
RUN bundle install
RUN rails db:migrate
CMD rails s