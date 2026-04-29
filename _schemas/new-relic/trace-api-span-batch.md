---
description: A batch of spans with optional shared attributes
layout: schema
name: SpanBatch
properties_list:
- description: ''
  name: common
  type: object
- description: Array of individual span objects
  name: spans
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/trace-api-span-batch-schema.json
slug: trace-api-span-batch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-span-batch-schema.json\",\n  \"title\": \"SpanBatch\",\n  \"description\": \"A batch of spans with optional shared attributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"common\": {\n      \"$ref\": \"#/components/schemas/CommonBlock\"\n    },\n    \"spans\": {\n      \"type\": \"array\",\n      \"description\": \"Array of individual span objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Span\"\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"trace.id\": \"500123\",\n          \"timestamp\": 1718153645993,\n          \"attributes\": {\n            \"name\": {},\n            \"parent.id\": {},\n            \"duration.ms\": {},\n            \"service.name\": {},\n            \"error\": {},\n            \"db.statement\": {},\n  \
  \          \"http.url\": {},\n            \"http.method\": {},\n            \"http.statusCode\": {}\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spans\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-span-batch-schema.json
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
