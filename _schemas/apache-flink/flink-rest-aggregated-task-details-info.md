---
description: AggregatedTaskDetailsInfo schema from Apache Flink REST API
layout: schema
name: AggregatedTaskDetailsInfo
properties_list:
- description: ''
  name: metrics
  type: object
- description: ''
  name: status-duration
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-aggregated-task-details-info-schema.json
slug: flink-rest-aggregated-task-details-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-aggregated-task-details-info-schema.json\",\n  \"title\": \"AggregatedTaskDetailsInfo\",\n  \"description\": \"AggregatedTaskDetailsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"status-duration\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-aggregated-task-details-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: AggregatedTaskDetailsInfo
---
