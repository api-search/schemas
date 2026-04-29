---
description: ''
layout: schema
name: Condition
properties_list:
- description: ''
  name: condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-condition-schema.json
slug: new-relic-condition
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"condition_scope\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"entities\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"gc_metric\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"metric\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"terms\": {\n          \"type\": \"array\",\n          \"example\": [\n            {\n           \
  \   \"duration\": \"example_string\",\n              \"operator\": \"example_string\",\n              \"priority\": \"example_string\",\n              \"threshold\": \"example_string\",\n              \"time_function\": \"example_string\"\n            }\n          ],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"duration\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"operator\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"priority\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"threshold\": {\n                \"type\": \"string\",\n                \"example\": \"example_string\"\n              },\n              \"time_function\": {\n                \"type\": \"string\",\n                \"\
  example\": \"example_string\"\n              }\n            }\n          }\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"user_defined\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"metric\": {\n              \"type\": \"string\",\n              \"example\": \"example_string\"\n            },\n            \"value_function\": {\n              \"type\": \"string\",\n              \"example\": \"example_string\"\n            }\n          }\n        },\n        \"violation_close_timer\": {\n          \"type\": \"integer\",\n          \"example\": 1718153645993\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Condition\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-condition-schema.json
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
title: Condition
---
