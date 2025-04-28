ARG ELK_VERSION

FROM docker.elastic.co/beats/filebeat:${ELK_VERSION}

COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root

RUN mkdir /var/logs

RUN chmod go-w /usr/share/filebeat/filebeat.yml

RUN chown -R root /usr/share/filebeat
