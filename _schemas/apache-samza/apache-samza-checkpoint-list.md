---
description: List of checkpoints for a job
layout: schema
name: CheckpointList
properties_list:
- description: ''
  name: checkpoints
  type: array
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-checkpoint-list-schema.json
slug: apache-samza-checkpoint-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-checkpoint-list-schema.json\",\n  \"title\": \"CheckpointList\",\n  \"description\": \"List of checkpoints for a job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Checkpoint\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-checkpoint-list-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: CheckpointList
---
