---
description: ConnectorInfo schema from Apache kafka
layout: schema
name: ConnectorInfo
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: config
  type: object
- description: ''
  name: tasks
  type: array
- description: ''
  name: type
  type: string
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-connector-info-schema.json
slug: kafka-connect-connector-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-connector-info-schema.json\",\n  \"title\": \"ConnectorInfo\",\n  \"description\": \"ConnectorInfo schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"connector\": {\n            \"type\": \"string\"\n          },\n          \"task\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"source\",\n        \"sink\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-connector-info-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ConnectorInfo
---
