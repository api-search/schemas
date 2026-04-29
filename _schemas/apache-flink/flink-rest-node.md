---
description: Node schema from Apache Flink REST API
layout: schema
name: Node
properties_list:
- description: ''
  name: children
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-node-schema.json
slug: flink-rest-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-node-schema.json\",\n  \"title\": \"Node\",\n  \"description\": \"Node schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"children\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Node\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-node-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: Node
---
