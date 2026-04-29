---
description: ''
layout: schema
name: UserDefinedConditionBody
properties_list:
- description: ''
  name: metric
  type: string
- description: ''
  name: value_function
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-user-defined-condition-body-schema.json
slug: new-relic-user-defined-condition-body
source_filename: new-relic-user-defined-condition-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"value_function\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserDefinedConditionBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-user-defined-condition-body-schema.json
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
title: UserDefinedConditionBody
---
