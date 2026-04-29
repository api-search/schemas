---
description: Response statistics for a service.
layout: schema
name: ServiceStatistics
properties_list:
- description: ''
  name: OkCount
  type: object
- description: ''
  name: ErrorStatistics
  type: object
- description: ''
  name: FaultStatistics
  type: object
- description: ''
  name: TotalCount
  type: object
- description: ''
  name: TotalResponseTime
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-service-statistics-schema.json
slug: xray-service-statistics
source_filename: xray-service-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"OkCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of requests that completed with a 2xx Success status code.\"\n        }\n      ]\n    },\n    \"ErrorStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorStatistics\"\n        },\n        {\n          \"description\": \"Information about requests that failed with a 4xx Client Error status code.\"\n        }\n      ]\n    },\n    \"FaultStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FaultStatistics\"\n        },\n        {\n          \"description\": \"Information about requests that failed with a 5xx Server Error status code.\"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n  \
  \      },\n        {\n          \"description\": \"The total number of completed requests.\"\n        }\n      ]\n    },\n    \"TotalResponseTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The aggregate response time of completed requests.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Response statistics for a service.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-service-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-service-statistics-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ServiceStatistics
---
