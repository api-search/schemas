---
description: Label schema
layout: schema
name: Label
properties_list:
- description: ''
  name: label
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-label-schema.json
slug: openapi-label
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-schema.json\",\n  \"title\": \"Label\",\n  \"description\": \"Label schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"$ref\": \"#/components/schemas/LabelBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-schema.json
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
title: Label
---
