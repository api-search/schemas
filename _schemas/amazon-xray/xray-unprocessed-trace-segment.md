---
description: Information about a segment that failed processing.
layout: schema
name: UnprocessedTraceSegment
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-unprocessed-trace-segment-schema.json
slug: xray-unprocessed-trace-segment
source_filename: xray-unprocessed-trace-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The segment's ID.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error that caused processing to fail.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about a segment that failed processing.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnprocessedTraceSegment\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-unprocessed-trace-segment-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-unprocessed-trace-segment-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UnprocessedTraceSegment
---
