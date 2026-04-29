---
description: CreateTopicRequest schema from Apache kafka
layout: schema
name: CreateTopicRequest
properties_list:
- description: ''
  name: topic_name
  type: string
- description: ''
  name: partitions_count
  type: integer
- description: ''
  name: replication_factor
  type: integer
- description: ''
  name: configs
  type: array
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-create-topic-request-schema.json
slug: kafka-rest-proxy-create-topic-request
source_filename: kafka-rest-proxy-create-topic-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-create-topic-request-schema.json\",\n  \"title\": \"CreateTopicRequest\",\n  \"description\": \"CreateTopicRequest schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic_name\": {\n      \"type\": \"string\"\n    },\n    \"partitions_count\": {\n      \"type\": \"integer\"\n    },\n    \"replication_factor\": {\n      \"type\": \"integer\"\n    },\n    \"configs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"topic_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-create-topic-request-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: CreateTopicRequest
---
