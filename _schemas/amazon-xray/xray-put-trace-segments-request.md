---
description: PutTraceSegmentsRequest schema from Amazon X-Ray API
layout: schema
name: PutTraceSegmentsRequest
properties_list:
- description: ''
  name: TraceSegmentDocuments
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-put-trace-segments-request-schema.json
slug: xray-put-trace-segments-request
source_filename: xray-put-trace-segments-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"TraceSegmentDocuments\"\n  ],\n  \"title\": \"PutTraceSegmentsRequest\",\n  \"properties\": {\n    \"TraceSegmentDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceSegmentDocumentList\"\n        },\n        {\n          \"description\": \"A string containing a JSON document defining one or more segments or subsegments.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-trace-segments-request-schema.json\",\n  \"description\": \"PutTraceSegmentsRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-trace-segments-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: PutTraceSegmentsRequest
---
