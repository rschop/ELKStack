FROM docker.elastic.co/beats/metricbeat:7.10.0

LABEL maintainer="RSchop" \
      description="Metricbeat Risc"

COPY metricbeat.yml /usr/share/metricbeat/metricbeat.yml
USER root
RUN chown root:metricbeat /usr/share/metricbeat/metricbeat.yml
USER metricbeat