---
description: Topic schema from Apache kafka
layout: schema
name: Topic
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: cluster_id
  type: string
- description: ''
  name: topic_name
  type: string
- description: ''
  name: is_internal
  type: boolean
- description: ''
  name: replication_factor
  type: integer
- description: ''
  name: partitions_count
  type: integer
- description: ''
  name: partitions
  type: object
- description: ''
  name: configs
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-topic-schema.json
slug: kafka-rest-proxy-topic
source_filename: kafka-rest-proxy-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-topic-schema.json\",\n  \"title\": \"Topic\",\n  \"description\": \"Topic schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"topic_name\": {\n      \"type\": \"string\"\n    },\n    \"is_internal\": {\n      \"type\": \"boolean\"\n    },\n    \"replication_factor\": {\n      \"type\": \"integer\"\n    },\n    \"partitions_count\": {\n      \"type\": \"integer\"\n    },\n    \"partitions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"related\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"configs\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"related\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-topic-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Topic
---
