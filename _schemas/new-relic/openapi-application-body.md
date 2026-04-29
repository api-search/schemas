---
description: ApplicationBody schema
layout: schema
name: ApplicationBody
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: settings
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-body-schema.json
slug: openapi-application-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-body-schema.json\",\n  \"title\": \"ApplicationBody\",\n  \"description\": \"ApplicationBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"settings\": {\n      \"$ref\": \"#/components/schemas/AppSettingsBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-body-schema.json
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
title: ApplicationBody
---
