---
description: ConnectorStatus schema from Apache kafka
layout: schema
name: ConnectorStatus
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: connector
  type: object
- description: ''
  name: tasks
  type: array
- description: ''
  name: type
  type: string
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-connector-status-schema.json
slug: kafka-connect-connector-status
source_filename: kafka-connect-connector-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-connector-status-schema.json\",\n  \"title\": \"ConnectorStatus\",\n  \"description\": \"ConnectorStatus schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"connector\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"UNASSIGNED\",\n            \"RUNNING\",\n            \"PAUSED\",\n            \"FAILED\",\n            \"STOPPED\"\n          ]\n        },\n        \"worker_id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskStatus\"\n      }\n    },\n    \"type\": {\n      \"type\": \"\
  string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-connector-status-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ConnectorStatus
---
