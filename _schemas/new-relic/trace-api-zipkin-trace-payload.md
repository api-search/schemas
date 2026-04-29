---
description: Zipkin JSON v2 format trace payload
layout: schema
name: ZipkinTracePayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/trace-api-zipkin-trace-payload-schema.json
slug: trace-api-zipkin-trace-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-zipkin-trace-payload-schema.json\",\n  \"title\": \"ZipkinTracePayload\",\n  \"description\": \"Zipkin JSON v2 format trace payload\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ZipkinSpan\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-zipkin-trace-payload-schema.json
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
title: ZipkinTracePayload
---
