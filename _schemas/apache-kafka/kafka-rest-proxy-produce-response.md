---
description: ProduceResponse schema from Apache kafka
layout: schema
name: ProduceResponse
properties_list:
- description: ''
  name: error_code
  type: integer
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
  name: offset
  type: integer
- description: ''
  name: timestamp
  type: string
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-produce-response-schema.json
slug: kafka-rest-proxy-produce-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-produce-response-schema.json\",\n  \"title\": \"ProduceResponse\",\n  \"description\": \"ProduceResponse schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_code\": {\n      \"type\": \"integer\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"topic_name\": {\n      \"type\": \"string\"\n    },\n    \"partition_id\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-produce-response-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ProduceResponse
---
