---
description: List of Samza tasks
layout: schema
name: TaskList
properties_list:
- description: ''
  name: tasks
  type: array
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-task-list-schema.json
slug: apache-samza-task-list
source_filename: apache-samza-task-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-task-list-schema.json\",\n  \"title\": \"TaskList\",\n  \"description\": \"List of Samza tasks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Task\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-task-list-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: TaskList
---
