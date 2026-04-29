---
description: Checkpoint for a Samza task
layout: schema
name: Checkpoint
properties_list:
- description: Task name
  name: taskName
  type: string
- description: System stream partition identifier
  name: systemStreamPartition
  type: string
- description: Checkpoint offset value
  name: offset
  type: string
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-checkpoint-schema.json
slug: apache-samza-checkpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-checkpoint-schema.json\",\n  \"title\": \"Checkpoint\",\n  \"description\": \"Checkpoint for a Samza task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskName\": {\n      \"type\": \"string\",\n      \"description\": \"Task name\"\n    },\n    \"systemStreamPartition\": {\n      \"type\": \"string\",\n      \"description\": \"System stream partition identifier\"\n    },\n    \"offset\": {\n      \"type\": \"string\",\n      \"description\": \"Checkpoint offset value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-checkpoint-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Checkpoint
---
