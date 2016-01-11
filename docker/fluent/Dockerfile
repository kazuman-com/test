FROM fluent/fluentd:latest
MAINTAINER Takakazu Kaneko <hoge@hoge.jp>
USER fluent
WORKDIR /home/fluent
ENV PATH /home/fluent/.gem/ruby/2.2.0/bin:$PATH
RUN fluent-gem install fluent-plugin-mongo
CMD fluentd -c /fluentd/etc/$FLUENTD_CONF -p /fluentd/plugins $FLUENTD_OPT
