---
description: ''
layout: schema
name: ServiceStatistics
properties_list:
- description: ''
  name: OkCount
  type: integer
- description: ''
  name: ErrorStatistics
  type: object
- description: ''
  name: FaultStatistics
  type: object
- description: ''
  name: TotalCount
  type: integer
- description: ''
  name: TotalResponseTime
  type: number
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-servicestatistics-schema.json
slug: x-ray-servicestatistics
source_filename: x-ray-servicestatistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OkCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"ErrorStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ThrottleCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"OtherCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"FaultStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OtherCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"TotalCount\":\
  \ {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"TotalResponseTime\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-servicestatistics-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: ServiceStatistics
---
