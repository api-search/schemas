---
description: Condition schema
layout: schema
name: Condition
properties_list:
- description: ''
  name: condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-condition-schema.json
slug: openapi-condition
source_filename: openapi-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-condition-schema.json\",\n  \"title\": \"Condition\",\n  \"description\": \"Condition schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"$ref\": \"#/components/schemas/ConditionBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-condition-schema.json
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
