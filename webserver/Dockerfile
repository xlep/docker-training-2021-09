FROM ubuntu:20.04

RUN apt-get update \
    && apt-get install -yqq nginx


COPY nginx.conf /etc/nginx/sites-enabled/website
COPY startup.sh /startup.sh

RUN chmod +x /startup.sh

EXPOSE 80
EXPOSE 81

VOLUME ["/content"]

CMD ["/startup.sh"]

