# base image
FROM python:3.7.9

# author
MAINTAINER doubletrey doubletrey@163.com

# environment
#ENV APP_DIR=/app
ENV CRAWL_ENV=prod

ADD . /app
WORKDIR /app
COPY ./scrapyd.conf /etc/scrapyd/
RUN pip install -r requirements.txt && mkdir -p /logs
CMD scrapyd
