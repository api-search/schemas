---
description: LabelBody schema
layout: schema
name: LabelBody
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-label-body-schema.json
slug: openapi-label-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-body-schema.json\",\n  \"title\": \"LabelBody\",\n  \"description\": \"LabelBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/LabelLinksBody\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-body-schema.json
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
title: LabelBody
---
