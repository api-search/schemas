---
description: IncidentResponse schema
layout: schema
name: IncidentResponse
properties_list:
- description: ''
  name: incident
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-incident-response-schema.json
slug: openapi-incident-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-response-schema.json\",\n  \"title\": \"IncidentResponse\",\n  \"description\": \"IncidentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident\": {\n      \"$ref\": \"#/components/schemas/IncidentResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-response-schema.json
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
title: IncidentResponse
---
