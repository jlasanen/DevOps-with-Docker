# exercise 1.14
FROM ruby:2.6.0

CMD /bin/bash

# install node
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs

# install bundler
RUN gem install bundler

# get project
RUN git clone https://github.com/docker-hy/rails-example-project.git
WORKDIR rails-example-project

# install dependencies
RUN bundle install

# run project (in developer mode, because there were problems with production mode)
RUN rails db:migrate 
#RUN rake assets:precompile
CMD rails s


