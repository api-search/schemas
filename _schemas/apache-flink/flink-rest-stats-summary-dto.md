---
description: StatsSummaryDto schema from Apache Flink REST API
layout: schema
name: StatsSummaryDto
properties_list:
- description: ''
  name: avg
  type: integer
- description: ''
  name: max
  type: integer
- description: ''
  name: min
  type: integer
- description: ''
  name: p50
  type: number
- description: ''
  name: p90
  type: number
- description: ''
  name: p95
  type: number
- description: ''
  name: p99
  type: number
- description: ''
  name: p999
  type: number
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-stats-summary-dto-schema.json
slug: flink-rest-stats-summary-dto
source_filename: flink-rest-stats-summary-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-stats-summary-dto-schema.json\",\n  \"title\": \"StatsSummaryDto\",\n  \"description\": \"StatsSummaryDto schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"avg\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"max\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"min\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"p50\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"p90\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"p95\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"p99\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"p999\": {\n      \"type\": \"\
  number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-stats-summary-dto-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: StatsSummaryDto
---
