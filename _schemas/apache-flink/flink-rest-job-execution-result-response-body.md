---
description: JobExecutionResultResponseBody schema from Apache Flink REST API
layout: schema
name: JobExecutionResultResponseBody
properties_list:
- description: ''
  name: job-execution-result
  type: object
- description: ''
  name: status
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-execution-result-response-body-schema.json
slug: flink-rest-job-execution-result-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-execution-result-response-body-schema.json\",\n  \"title\": \"JobExecutionResultResponseBody\",\n  \"description\": \"JobExecutionResultResponseBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job-execution-result\": {\n      \"$ref\": \"#/components/schemas/JobResult\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/QueueStatus\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-execution-result-response-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobExecutionResultResponseBody
---
