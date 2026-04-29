---
description: Parallelism schema from Apache Flink REST API
layout: schema
name: Parallelism
properties_list:
- description: ''
  name: lowerBound
  type: integer
- description: ''
  name: upperBound
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-parallelism-schema.json
slug: flink-rest-parallelism
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-parallelism-schema.json\",\n  \"title\": \"Parallelism\",\n  \"description\": \"Parallelism schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lowerBound\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"upperBound\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-parallelism-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: Parallelism
---
