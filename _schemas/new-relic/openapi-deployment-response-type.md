---
description: DeploymentResponseType schema
layout: schema
name: DeploymentResponseType
properties_list:
- description: ''
  name: changelog
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: links
  type: object
- description: ''
  name: revision
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: user
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-deployment-response-type-schema.json
slug: openapi-deployment-response-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-response-type-schema.json\",\n  \"title\": \"DeploymentResponseType\",\n  \"description\": \"DeploymentResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"changelog\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/DeploymentLinksResponse\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"user\": {\n      \"\
  type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-response-type-schema.json
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
title: DeploymentResponseType
---
