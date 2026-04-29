---
description: Metric schema from Apache Flink REST API
layout: schema
name: Metric
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: value
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-metric-schema.json
slug: flink-rest-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"Metric schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-metric-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: Metric
---
