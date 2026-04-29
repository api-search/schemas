---
description: JobVertexAccumulatorsInfo schema from Apache Flink REST API
layout: schema
name: JobVertexAccumulatorsInfo
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: user-accumulators
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-vertex-accumulators-info-schema.json
slug: flink-rest-job-vertex-accumulators-info
source_filename: flink-rest-job-vertex-accumulators-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-accumulators-info-schema.json\",\n  \"title\": \"JobVertexAccumulatorsInfo\",\n  \"description\": \"JobVertexAccumulatorsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"user-accumulators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserAccumulator\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-accumulators-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobVertexAccumulatorsInfo
---
