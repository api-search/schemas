---
description: Statistics that describe how the incident has impacted a service.
layout: schema
name: RequestImpactStatistics
properties_list:
- description: ''
  name: FaultCount
  type: object
- description: ''
  name: OkCount
  type: object
- description: ''
  name: TotalCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-request-impact-statistics-schema.json
slug: xray-request-impact-statistics
source_filename: xray-request-impact-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FaultCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of requests that have resulted in a fault,\"\n        }\n      ]\n    },\n    \"OkCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of successful requests.\"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The total number of requests to the service.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Statistics that describe how the incident has impacted a service.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestImpactStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-request-impact-statistics-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-request-impact-statistics-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: RequestImpactStatistics
---
