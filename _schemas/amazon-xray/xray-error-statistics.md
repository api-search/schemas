---
description: Information about requests that failed with a 4xx Client Error status code.
layout: schema
name: ErrorStatistics
properties_list:
- description: ''
  name: ThrottleCount
  type: object
- description: ''
  name: OtherCount
  type: object
- description: ''
  name: TotalCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-error-statistics-schema.json
slug: xray-error-statistics
source_filename: xray-error-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ThrottleCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of requests that failed with a 419 throttling status code.\"\n        }\n      ]\n    },\n    \"OtherCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The number of requests that failed with untracked 4xx Client Error status codes.\"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The total number of requests that failed with a 4xx Client Error status code.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about requests that failed with a 4xx Client Error status code.\",\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-error-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-error-statistics-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ErrorStatistics
---
