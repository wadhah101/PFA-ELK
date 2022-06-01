ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELASTIC_VERSION}

ADD config/elasticsearch.yml /usr/share/elasticsearch/config/
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu

RUN curl -X PUT "localhost:9200/cortex_6?pretty"