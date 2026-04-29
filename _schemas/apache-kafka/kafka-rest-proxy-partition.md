---
description: Partition schema from Apache kafka
layout: schema
name: Partition
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
  name: partition_id
  type: integer
- description: ''
  name: leader
  type: object
- description: ''
  name: replicas
  type: array
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-partition-schema.json
slug: kafka-rest-proxy-partition
source_filename: kafka-rest-proxy-partition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-partition-schema.json\",\n  \"title\": \"Partition\",\n  \"description\": \"Partition schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"topic_name\": {\n      \"type\": \"string\"\n    },\n    \"partition_id\": {\n      \"type\": \"integer\"\n    },\n    \"leader\": {\n      \"type\": \"object\"\n    },\n    \"replicas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-partition-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Partition
---
