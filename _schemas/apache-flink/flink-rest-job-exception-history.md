---
description: JobExceptionHistory schema from Apache Flink REST API
layout: schema
name: JobExceptionHistory
properties_list:
- description: ''
  name: entries
  type: array
- description: ''
  name: truncated
  type: boolean
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-exception-history-schema.json
slug: flink-rest-job-exception-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-exception-history-schema.json\",\n  \"title\": \"JobExceptionHistory\",\n  \"description\": \"JobExceptionHistory schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RootExceptionInfo\"\n      }\n    },\n    \"truncated\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-exception-history-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobExceptionHistory
---
