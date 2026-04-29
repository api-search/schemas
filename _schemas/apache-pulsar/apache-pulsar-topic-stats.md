---
description: TopicStats schema from Apache Pulsar
layout: schema
name: TopicStats
properties_list:
- description: ''
  name: msgRateIn
  type: number
- description: ''
  name: msgRateOut
  type: number
- description: ''
  name: msgThroughputIn
  type: number
- description: ''
  name: msgThroughputOut
  type: number
- description: ''
  name: averageMsgSize
  type: number
- description: ''
  name: storageSize
  type: integer
- description: ''
  name: backlogSize
  type: integer
- description: ''
  name: publishers
  type: array
- description: ''
  name: subscriptions
  type: object
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-topic-stats-schema.json
slug: apache-pulsar-topic-stats
source_filename: apache-pulsar-topic-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-topic-stats-schema.json\",\n  \"title\": \"TopicStats\",\n  \"description\": \"TopicStats schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"msgRateIn\": {\n      \"type\": \"number\"\n    },\n    \"msgRateOut\": {\n      \"type\": \"number\"\n    },\n    \"msgThroughputIn\": {\n      \"type\": \"number\"\n    },\n    \"msgThroughputOut\": {\n      \"type\": \"number\"\n    },\n    \"averageMsgSize\": {\n      \"type\": \"number\"\n    },\n    \"storageSize\": {\n      \"type\": \"integer\"\n    },\n    \"backlogSize\": {\n      \"type\": \"integer\"\n    },\n    \"publishers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"msgRateIn\": {\n            \"type\": \"number\"\n          },\n\
  \          \"msgThroughputIn\": {\n            \"type\": \"number\"\n          },\n          \"producerName\": {\n            \"type\": \"string\"\n          },\n          \"producerId\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"subscriptions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"msgRateOut\": {\n            \"type\": \"number\"\n          },\n          \"msgThroughputOut\": {\n            \"type\": \"number\"\n          },\n          \"msgBacklog\": {\n            \"type\": \"integer\"\n          },\n          \"consumers\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-topic-stats-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TopicStats
---
