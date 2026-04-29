---
description: ''
layout: schema
name: NrqlResponse
properties_list:
- description: ''
  name: query
  type: string
- description: ''
  name: since_value
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-nrql-response-schema.json
slug: new-relic-nrql-response
source_filename: new-relic-nrql-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"since_value\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NrqlResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-nrql-response-schema.json
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
title: NrqlResponse
---
