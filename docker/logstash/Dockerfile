FROM docker.elastic.co/logstash/logstash:5.3.0

RUN apt-get update && apt-get install -y build-essential
RUN apt-get install -y --no-install-recommends \
    vim \
    less \
    pkg-config \
    telnet

# add custom config
COPY docker/logstash/logstash.conf /config-dir/logstash.conf

# add templates
COPY docker/logstash/templates/ /config-dir/templates/

EXPOSE 5044
