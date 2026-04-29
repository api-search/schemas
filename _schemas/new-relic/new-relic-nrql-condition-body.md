---
description: ''
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
schema_file: json-schema/new-relic-nrql-condition-body-schema.json
slug: new-relic-nrql-condition-body
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"expected_groups\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"ignore_overlap\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"nrql\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"query\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"since_value\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        }\n      }\n    },\n    \"runbook_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://portal.example.com/path/abc123\"\n    },\n    \"terms\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"duration\": \"example_string\",\n          \"operator\"\
  : \"example_string\",\n          \"priority\": \"example_string\",\n          \"threshold\": \"example_string\",\n          \"time_function\": \"example_string\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"priority\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"threshold\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"time_function\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          }\n        }\n      }\n    },\n    \"value_function\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n\
  \  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NrqlConditionBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-nrql-condition-body-schema.json
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
