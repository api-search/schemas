---
description: Information about requests that failed with a 5xx Server Error status code.
layout: schema
name: FaultStatistics
properties_list:
- description: ''
  name: OtherCount
  type: object
- description: ''
  name: TotalCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-fault-statistics-schema.json
slug: xray-fault-statistics
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"OtherCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of requests that failed with untracked 5xx Server Error status codes.\"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The total number of requests that failed with a 5xx Server Error status code.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about requests that failed with a 5xx Server Error status code.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FaultStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-fault-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-fault-statistics-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: FaultStatistics
---
