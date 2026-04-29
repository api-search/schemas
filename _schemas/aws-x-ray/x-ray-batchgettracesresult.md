---
description: ''
layout: schema
name: BatchGetTracesResult
properties_list:
- description: ''
  name: Traces
  type: array
- description: ''
  name: UnprocessedTraceIds
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-batchgettracesresult-schema.json
slug: x-ray-batchgettracesresult
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchGetTracesResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Traces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the request that generated the trace.\"\n          },\n          \"Duration\": {\n            \"type\": \"number\",\n            \"description\": \"The length of time in seconds between the start and end times.\"\n          },\n          \"LimitExceeded\": {\n            \"type\": \"boolean\"\n          },\n          \"Segments\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"string\"\n                },\n                \"Document\": {\n        \
  \          \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"UnprocessedTraceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-batchgettracesresult-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: BatchGetTracesResult
---
