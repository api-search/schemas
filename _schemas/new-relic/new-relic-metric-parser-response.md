---
description: ''
layout: schema
name: MetricParserResponse
properties_list:
- description: ''
  name: metric
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-metric-parser-response-schema.json
slug: new-relic-metric-parser-response
source_filename: new-relic-metric-parser-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"values\": {\n          \"type\": \"array\",\n          \"example\": [\n            \"example_string\"\n          ],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricParserResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-parser-response-schema.json
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
