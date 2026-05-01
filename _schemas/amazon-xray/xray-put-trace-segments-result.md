---
description: PutTraceSegmentsResult schema from Amazon X-Ray API
layout: schema
name: PutTraceSegmentsResult
properties_list:
- description: ''
  name: UnprocessedTraceSegments
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-put-trace-segments-result-schema.json
slug: xray-put-trace-segments-result
source_filename: xray-put-trace-segments-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedTraceSegments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedTraceSegmentList\"\n        },\n        {\n          \"description\": \"Segments that failed processing.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutTraceSegmentsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-trace-segments-result-schema.json\",\n  \"description\": \"PutTraceSegmentsResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-trace-segments-result-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: PutTraceSegmentsResult
---
