ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/kibana/kibana:${ELK_VERSION}

# Add your kibana plugins setup here
# Example: RUN kibana-plugin install <name|url>
RUN kibana-plugin install https://github.com/fbaligand/kibana-enhanced-table/releases/download/v1.14.0/enhanced-table-1.14.0_8.17.3.zip
