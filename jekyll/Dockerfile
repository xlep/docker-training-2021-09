FROM ruby:3.0.2

RUN gem install jekyll bundler

COPY startup.sh /startup.sh
RUN chmod +x startup.sh

VOLUME ["/input"]
VOLUME ["/output"]

WORKDIR /input/
CMD ["/startup.sh"]
