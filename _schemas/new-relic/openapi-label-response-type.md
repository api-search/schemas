---
description: LabelResponseType schema
layout: schema
name: LabelResponseType
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: origins
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-label-response-type-schema.json
slug: openapi-label-response-type
source_filename: openapi-label-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-response-type-schema.json\",\n  \"title\": \"LabelResponseType\",\n  \"description\": \"LabelResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/LabelLinksResponse\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"origins\": {\n      \"$ref\": \"#/components/schemas/LabelOriginsResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-response-type-schema.json
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
title: LabelResponseType
---
