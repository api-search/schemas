---
description: PolicyBody schema
layout: schema
name: PolicyBody
properties_list:
- description: ''
  name: incident_preference
  type: string
- description: ''
  name: name
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-policy-body-schema.json
slug: openapi-policy-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-body-schema.json\",\n  \"title\": \"PolicyBody\",\n  \"description\": \"PolicyBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident_preference\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-body-schema.json
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
title: PolicyBody
---
