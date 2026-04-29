---
description: TaskInfo schema from Apache kafka
layout: schema
name: TaskInfo
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: config
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-task-info-schema.json
slug: kafka-connect-task-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-task-info-schema.json\",\n  \"title\": \"TaskInfo\",\n  \"description\": \"TaskInfo schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"connector\": {\n          \"type\": \"string\"\n        },\n        \"task\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-task-info-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: TaskInfo
---
