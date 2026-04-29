---
description: MetricParserResponse schema
layout: schema
name: MetricParserResponse
properties_list:
- description: ''
  name: metric
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-metric-parser-response-schema.json
slug: openapi-metric-parser-response
source_filename: openapi-metric-parser-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-parser-response-schema.json\",\n  \"title\": \"MetricParserResponse\",\n  \"description\": \"MetricParserResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"$ref\": \"#/components/schemas/MetricParserResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-parser-response-schema.json
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
title: MetricParserResponse
---
