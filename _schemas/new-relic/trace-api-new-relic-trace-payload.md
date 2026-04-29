---
description: New Relic format trace payload — array of span batch objects
layout: schema
name: NewRelicTracePayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/trace-api-new-relic-trace-payload-schema.json
slug: trace-api-new-relic-trace-payload
source_filename: trace-api-new-relic-trace-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-new-relic-trace-payload-schema.json\",\n  \"title\": \"NewRelicTracePayload\",\n  \"description\": \"New Relic format trace payload \\u2014 array of span batch objects\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SpanBatch\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-new-relic-trace-payload-schema.json
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
title: NewRelicTracePayload
---
