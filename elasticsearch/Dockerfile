ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
# 한글형태소 분석기
RUN elasticsearch-plugin install analysis-nori
# 다국어 검색에 유용한 더 나은 유니 코드 텍스트 분석을 제공
RUN elasticsearch/bin/elasticsearch-plugin install analysis-icu
# 다양한 문서 형식 (PDF, DOCX 등)에서 텍스트와 메타 데이터를 추출
RUN elasticsearch/bin/elasticsearch-plugin install ingest-attachment
# 문서 크기를 저장하고 검색하는 기능을 추가
RUN elasticsearch/bin/elasticsearch-plugin install mapper-size
# 필드 값에 대한 해시를 생성
RUN elasticsearch/bin/elasticsearch-plugin install mapper-murmur3
# Elasticsearch 클러스터에 대한 AWS EC2 기반 발견에 도움
RUN elasticsearch/bin/elasticsearch-plugin install discovery-ec2
