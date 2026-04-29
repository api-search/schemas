---
description: A single distributed trace span in New Relic format
layout: schema
name: Span
properties_list:
- description: Unique identifier for this span (16 hex characters)
  name: id
  type: string
- description: Trace ID that groups all spans in a distributed trace
  name: trace.id
  type: string
- description: Unix epoch timestamp in milliseconds when the span started
  name: timestamp
  type: integer
- description: Span attributes
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/trace-api-span-schema.json
slug: trace-api-span
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-span-schema.json\",\n  \"title\": \"Span\",\n  \"description\": \"A single distributed trace span in New Relic format\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this span (16 hex characters)\",\n      \"example\": \"500123\"\n    },\n    \"trace.id\": {\n      \"type\": \"string\",\n      \"description\": \"Trace ID that groups all spans in a distributed trace\",\n      \"example\": \"500123\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds when the span started\",\n      \"example\": 1718153645993\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Span attributes\",\n      \"properties\": {\n\
  \        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the operation represented by this span\"\n        },\n        \"parent.id\": {\n          \"type\": \"string\",\n          \"description\": \"The span ID of the parent span\"\n        },\n        \"duration.ms\": {\n          \"type\": \"number\",\n          \"description\": \"Duration of the span in milliseconds\"\n        },\n        \"service.name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the service that generated this span\"\n        },\n        \"error\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the span represents an error\"\n        },\n        \"db.statement\": {\n          \"type\": \"string\",\n          \"description\": \"Database query statement if applicable\"\n        },\n        \"http.url\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP URL for outbound calls\"\n        },\n        \"http.method\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for outbound calls\"\n        },\n        \"http.statusCode\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTP response status code\"\n        }\n      },\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      },\n      \"example\": {\n        \"name\": \"example-resource-01\",\n        \"parent.id\": \"500123\",\n        \"duration.ms\": 0.42,\n        \"service.name\": \"myService\",\n        \"error\": true,\n        \"db.statement\": \"example_string\",\n        \"http.url\": \"https://portal.example.com/path/abc123\",\n        \"http.method\": \"example_string\",\n        \"http.statusCode\": 200\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"trace.id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-span-schema.json
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
title: Span
---
