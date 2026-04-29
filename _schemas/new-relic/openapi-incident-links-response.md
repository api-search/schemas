---
description: IncidentLinksResponse schema
layout: schema
name: IncidentLinksResponse
properties_list:
- description: ''
  name: policy_id
  type: integer
- description: ''
  name: violations
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-incident-links-response-schema.json
slug: openapi-incident-links-response
source_filename: openapi-incident-links-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-links-response-schema.json\",\n  \"title\": \"IncidentLinksResponse\",\n  \"description\": \"IncidentLinksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"violations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-incident-links-response-schema.json
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
title: IncidentLinksResponse
---
