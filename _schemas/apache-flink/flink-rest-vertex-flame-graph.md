---
description: VertexFlameGraph schema from Apache Flink REST API
layout: schema
name: VertexFlameGraph
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: endTimestamp
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-vertex-flame-graph-schema.json
slug: flink-rest-vertex-flame-graph
source_filename: flink-rest-vertex-flame-graph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-vertex-flame-graph-schema.json\",\n  \"title\": \"VertexFlameGraph\",\n  \"description\": \"VertexFlameGraph schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/Node\"\n    },\n    \"endTimestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-vertex-flame-graph-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: VertexFlameGraph
---
