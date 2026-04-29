---
description: NrqlConditionBody schema
layout: schema
name: NrqlConditionBody
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: expected_groups
  type: integer
- description: ''
  name: ignore_overlap
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: nrql
  type: object
- description: ''
  name: runbook_url
  type: string
- description: ''
  name: terms
  type: array
- description: ''
  name: value_function
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-nrql-condition-body-schema.json
slug: openapi-nrql-condition-body
source_filename: openapi-nrql-condition-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-body-schema.json\",\n  \"title\": \"NrqlConditionBody\",\n  \"description\": \"NrqlConditionBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"expected_groups\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"ignore_overlap\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"nrql\": {\n      \"$ref\": \"#/components/schemas/NrqlBody\"\n    },\n    \"runbook_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    },\n    \"terms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\"\
  : \"#/components/schemas/IJKTermsType\"\n      },\n      \"example\": [\n        {\n          \"duration\": \"example_string\",\n          \"operator\": \"example_string\",\n          \"priority\": \"example_string\",\n          \"threshold\": \"example_string\",\n          \"time_function\": \"example_string\"\n        }\n      ]\n    },\n    \"value_function\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-body-schema.json
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
title: NrqlConditionBody
---
