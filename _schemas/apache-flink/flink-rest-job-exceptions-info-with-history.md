---
description: JobExceptionsInfoWithHistory schema from Apache Flink REST API
layout: schema
name: JobExceptionsInfoWithHistory
properties_list:
- description: ''
  name: exceptionHistory
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-exceptions-info-with-history-schema.json
slug: flink-rest-job-exceptions-info-with-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-exceptions-info-with-history-schema.json\",\n  \"title\": \"JobExceptionsInfoWithHistory\",\n  \"description\": \"JobExceptionsInfoWithHistory schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exceptionHistory\": {\n      \"$ref\": \"#/components/schemas/JobExceptionHistory\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-exceptions-info-with-history-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobExceptionsInfoWithHistory
---
