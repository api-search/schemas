---
description: ConsumerGroup schema from Apache kafka
layout: schema
name: ConsumerGroup
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
  name: consumer_group_id
  type: string
- description: ''
  name: is_simple
  type: boolean
- description: ''
  name: partition_assignor
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: coordinator
  type: object
- description: ''
  name: consumers
  type: object
- description: ''
  name: lag_summary
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-consumer-group-schema.json
slug: kafka-rest-proxy-consumer-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-consumer-group-schema.json\",\n  \"title\": \"ConsumerGroup\",\n  \"description\": \"ConsumerGroup schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"consumer_group_id\": {\n      \"type\": \"string\"\n    },\n    \"is_simple\": {\n      \"type\": \"boolean\"\n    },\n    \"partition_assignor\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UNKNOWN\",\n        \"PREPARING_REBALANCE\",\n        \"COMPLETING_REBALANCE\",\n        \"STABLE\",\n        \"DEAD\",\n        \"EMPTY\"\n      ]\n    },\n    \"coordinator\": {\n      \"\
  type\": \"object\"\n    },\n    \"consumers\": {\n      \"type\": \"object\"\n    },\n    \"lag_summary\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-consumer-group-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ConsumerGroup
---
