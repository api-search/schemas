---
description: A batch of spans with optional shared attributes
layout: schema
name: SpanBatch
properties_list:
- description: Shared attributes applied to all spans in this batch
  name: common
  type: object
- description: Array of individual span objects
  name: spans
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-trace-span-batch-schema.json
slug: new-relic-trace-span-batch
source_filename: new-relic-trace-span-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A batch of spans with optional shared attributes\",\n  \"properties\": {\n    \"common\": {\n      \"type\": \"object\",\n      \"description\": \"Shared attributes applied to all spans in this batch\",\n      \"properties\": {\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value attributes applied to every span in the batch\",\n          \"example\": {\n            \"customAttribute\": \"example_value\"\n          }\n        }\n      }\n    },\n    \"spans\": {\n      \"type\": \"array\",\n      \"description\": \"Array of individual span objects\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"trace.id\": \"500123\",\n          \"timestamp\": 1718153645993,\n          \"attributes\": {\n            \"name\": {},\n            \"parent.id\": {},\n            \"duration.ms\": {},\n            \"service.name\": {},\n            \"error\": {},\n      \
  \      \"db.statement\": {},\n            \"http.url\": {},\n            \"http.method\": {},\n            \"http.statusCode\": {}\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single distributed trace span in New Relic format\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for this span (16 hex characters)\",\n            \"example\": \"500123\"\n          },\n          \"trace.id\": {\n            \"type\": \"string\",\n            \"description\": \"Trace ID that groups all spans in a distributed trace\",\n            \"example\": \"500123\"\n          },\n          \"timestamp\": {\n            \"type\": \"integer\",\n            \"description\": \"Unix epoch timestamp in milliseconds when the span started\",\n            \"example\": 1718153645993\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n\
  \            \"description\": \"Span attributes\",\n            \"example\": {\n              \"name\": \"example-resource-01\",\n              \"parent.id\": \"500123\",\n              \"duration.ms\": 0.42,\n              \"service.name\": \"myService\",\n              \"error\": true,\n              \"db.statement\": \"example_string\",\n              \"http.url\": \"https://portal.example.com/path/abc123\",\n              \"http.method\": \"example_string\",\n              \"http.statusCode\": 200\n            },\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the operation represented by this span\"\n              },\n              \"parent.id\": {\n                \"type\": \"string\",\n                \"description\": \"The span ID of the parent span\"\n              },\n              \"duration.ms\": {\n                \"type\": \"number\",\n                \"description\": \"Duration of\
  \ the span in milliseconds\"\n              },\n              \"service.name\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the service that generated this span\"\n              },\n              \"error\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the span represents an error\"\n              },\n              \"db.statement\": {\n                \"type\": \"string\",\n                \"description\": \"Database query statement if applicable\"\n              },\n              \"http.url\": {\n                \"type\": \"string\",\n                \"description\": \"HTTP URL for outbound calls\"\n              },\n              \"http.method\": {\n                \"type\": \"string\",\n                \"description\": \"HTTP method for outbound calls\"\n              },\n              \"http.statusCode\": {\n                \"type\": \"integer\",\n                \"description\": \"HTTP response status\
  \ code\"\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"trace.id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"spans\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpanBatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-trace-span-batch-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: SpanBatch
---
