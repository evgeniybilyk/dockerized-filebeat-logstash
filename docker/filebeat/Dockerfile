FROM prima/filebeat:5.3

RUN apt-get update && apt-get install -y build-essential
RUN apt-get install -y --no-install-recommends \
    vim \
    less \
    pkg-config \
    telnet

COPY docker/filebeat/filebeat.yml /filebeat.yml
