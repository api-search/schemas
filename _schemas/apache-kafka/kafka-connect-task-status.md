---
description: TaskStatus schema from Apache kafka
layout: schema
name: TaskStatus
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: state
  type: string
- description: ''
  name: worker_id
  type: string
- description: ''
  name: trace
  type: string
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-task-status-schema.json
slug: kafka-connect-task-status
source_filename: kafka-connect-task-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-task-status-schema.json\",\n  \"title\": \"TaskStatus\",\n  \"description\": \"TaskStatus schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UNASSIGNED\",\n        \"RUNNING\",\n        \"PAUSED\",\n        \"FAILED\"\n      ]\n    },\n    \"worker_id\": {\n      \"type\": \"string\"\n    },\n    \"trace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-task-status-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: TaskStatus
---
