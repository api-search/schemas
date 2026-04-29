---
description: ''
layout: schema
name: NrqlConditionResponse
properties_list:
- description: ''
  name: nrql_condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-nrql-condition-response-schema.json
slug: new-relic-nrql-condition-response
source_filename: new-relic-nrql-condition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"nrql_condition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"expected_groups\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"ignore_overlap\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"nrql\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"query\": {\n              \"type\": \"string\",\n              \"example\": \"example_string\"\n            },\n            \"since_value\": {\n              \"type\": \"string\",\n              \"example\": \"example_string\"\n            }\n\
  \          }\n        },\n        \"runbook_url\": {\n          \"type\": \"string\",\n          \"example\": \"https://portal.example.com/path/abc123\"\n        },\n        \"terms\": {\n          \"type\": \"array\",\n          \"example\": [\n            {\n              \"duration\": \"example_string\",\n              \"operator\": \"example_string\",\n              \"priority\": \"example_string\",\n              \"threshold\": \"example_string\",\n              \"time_function\": \"example_string\"\n            }\n          ],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"duration\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"operator\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"priority\": {\n                \"type\": \"string\",\n                \"example\"\
  : \"example_string\"\n              },\n              \"threshold\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"time_function\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              }\n            }\n          }\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"value_function\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NrqlConditionResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-nrql-condition-response-schema.json
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
title: NrqlConditionResponse
---
