---
description: IncidentResponseType schema
layout: schema
name: IncidentResponseType
properties_list:
- description: ''
  name: closed_at
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: incident_preference
  type: integer
- description: ''
  name: links
  type: object
- description: ''
  name: opened_at
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-incident-response-type-schema.json
slug: openapi-incident-response-type
source_filename: openapi-incident-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-response-type-schema.json\",\n  \"title\": \"IncidentResponseType\",\n  \"description\": \"IncidentResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"closed_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"incident_preference\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/IncidentLinksResponse\"\n    },\n    \"opened_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-response-type-schema.json
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
title: IncidentResponseType
---
