---
description: ''
layout: schema
name: SyntheticsConditionResponseType
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: id
  type: integer
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
schema_file: json-schema/new-relic-synthetics-condition-response-type-schema.json
slug: new-relic-synthetics-condition-response-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"monitor_id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"runbook_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SyntheticsConditionResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-synthetics-condition-response-type-schema.json
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
title: SyntheticsConditionResponseType
---
