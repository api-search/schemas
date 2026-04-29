---
description: ''
layout: schema
name: Trace
properties_list:
- description: The unique identifier for the request that generated the trace.
  name: Id
  type: string
- description: The length of time in seconds between the start and end times.
  name: Duration
  type: number
- description: ''
  name: LimitExceeded
  type: boolean
- description: ''
  name: Segments
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-trace-schema.json
slug: x-ray-trace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Trace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the request that generated the trace.\"\n    },\n    \"Duration\": {\n      \"type\": \"number\",\n      \"description\": \"The length of time in seconds between the start and end times.\"\n    },\n    \"LimitExceeded\": {\n      \"type\": \"boolean\"\n    },\n    \"Segments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Id\": {\n            \"type\": \"string\"\n          },\n          \"Document\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-trace-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: Trace
---
