---
description: Error response
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: success
  type: boolean
- description: Error message
  name: error
  type: string
- description: List of validation errors
  name: errors
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-event-error-response-schema.json
slug: new-relic-event-error-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"example_string\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation errors\",\n      \"example\": [\n        {\n          \"error\": \"example_string\",\n          \"timestamp\": \"example_string\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"error\": {\n            \"type\": \"string\"\n          },\n          \"timestamp\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-event-error-response-schema.json
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
title: ErrorResponse
---
