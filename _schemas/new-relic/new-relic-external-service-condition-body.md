---
description: ''
layout: schema
name: ExternalServiceConditionBody
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: entities
  type: array
- description: ''
  name: external_service_url
  type: string
- description: ''
  name: metric
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: runbook_url
  type: string
- description: ''
  name: terms
  type: array
- description: ''
  name: type
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-external-service-condition-body-schema.json
slug: new-relic-external-service-condition-body
source_filename: new-relic-external-service-condition-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"entities\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"external_service_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"runbook_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    },\n    \"terms\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"duration\": \"example_string\",\n          \"operator\": \"example_string\",\n          \"priority\": \"example_string\",\n          \"threshold\": \"example_string\"\
  ,\n          \"time_function\": \"example_string\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"priority\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"threshold\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"time_function\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          }\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExternalServiceConditionBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-external-service-condition-body-schema.json
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
title: ExternalServiceConditionBody
---
