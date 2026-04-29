---
description: ApplicationResponseType schema
layout: schema
name: ApplicationResponseType
properties_list:
- description: ''
  name: application_summary
  type: object
- description: ''
  name: end_user_summary
  type: object
- description: ''
  name: health_status
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: language
  type: string
- description: ''
  name: last_reported_at
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: reporting
  type: boolean
- description: ''
  name: settings
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-response-type-schema.json
slug: openapi-application-response-type
source_filename: openapi-application-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-response-type-schema.json\",\n  \"title\": \"ApplicationResponseType\",\n  \"description\": \"ApplicationResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application_summary\": {\n      \"$ref\": \"#/components/schemas/AppSummaryResponse\"\n    },\n    \"end_user_summary\": {\n      \"$ref\": \"#/components/schemas/EndUserSummaryResponse\"\n    },\n    \"health_status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"last_reported_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"links\"\
  : {\n      \"$ref\": \"#/components/schemas/ApplicationLinksResponse\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"reporting\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"settings\": {\n      \"$ref\": \"#/components/schemas/AppSettingsResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-response-type-schema.json
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
title: ApplicationResponseType
---
