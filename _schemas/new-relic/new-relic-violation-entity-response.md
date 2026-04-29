---
description: ''
layout: schema
name: ViolationEntityResponse
properties_list:
- description: ''
  name: group_id
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: product
  type: string
- description: ''
  name: type
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-violation-entity-response-schema.json
slug: new-relic-violation-entity-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"group_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViolationEntityResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-violation-entity-response-schema.json
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
title: ViolationEntityResponse
---
