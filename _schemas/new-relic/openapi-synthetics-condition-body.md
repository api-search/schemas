---
description: SyntheticsConditionBody schema
layout: schema
name: SyntheticsConditionBody
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: monitor_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: runbook_url
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-synthetics-condition-body-schema.json
slug: openapi-synthetics-condition-body
source_filename: openapi-synthetics-condition-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-synthetics-condition-body-schema.json\",\n  \"title\": \"SyntheticsConditionBody\",\n  \"description\": \"SyntheticsConditionBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"monitor_id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"runbook_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-synthetics-condition-body-schema.json
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
title: SyntheticsConditionBody
---
