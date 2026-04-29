---
description: Samza task within a container
layout: schema
name: Task
properties_list:
- description: Task name
  name: taskName
  type: string
- description: Container the task runs on
  name: containerId
  type: string
- description: Task status
  name: status
  type: string
- description: ''
  name: partitions
  type: array
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-task-schema.json
slug: apache-samza-task
source_filename: apache-samza-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Samza task within a container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskName\": {\n      \"type\": \"string\",\n      \"description\": \"Task name\"\n    },\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"Container the task runs on\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Task status\"\n    },\n    \"partitions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Partition\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-task-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Task
---
