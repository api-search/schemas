---
description: JobStatusInfo schema from Apache Flink REST API
layout: schema
name: JobStatusInfo
properties_list:
- description: ''
  name: status
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-status-info-schema.json
slug: flink-rest-job-status-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-status-info-schema.json\",\n  \"title\": \"JobStatusInfo\",\n  \"description\": \"JobStatusInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/JobStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-status-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobStatusInfo
---
