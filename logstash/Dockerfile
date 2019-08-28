ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-input-jdbc
RUN logstash-plugin install logstash-output-elasticsearch
RUN logstash-plugin install logstash-filter-grok
RUN logstash-plugin install logstash-input-elasticsearch