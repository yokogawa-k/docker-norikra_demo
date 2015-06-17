FROM ruby:2.2
MAINTAINER Kazuya Yokogawa "yokogawa-k@klab.com"

COPY Gemfile.netflow /opt/netflow/Gemfile
RUN cd /opt/netflow \
 && bundle install

RUN gem install \
    fluentd \
    fluent-plugin-norikra \
    fluent-plugin-mackerel \
    fluent-plugin-flatten-hash
