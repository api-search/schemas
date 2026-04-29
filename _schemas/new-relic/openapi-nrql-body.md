---
description: NrqlBody schema
layout: schema
name: NrqlBody
properties_list:
- description: ''
  name: query
  type: string
- description: ''
  name: since_value
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-nrql-body-schema.json
slug: openapi-nrql-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-body-schema.json\",\n  \"title\": \"NrqlBody\",\n  \"description\": \"NrqlBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"since_value\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-body-schema.json
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
title: NrqlBody
---
