---
description: ''
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
schema_file: json-schema/new-relic-incident-response-type-schema.json
slug: new-relic-incident-response-type
source_filename: new-relic-incident-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"closed_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"incident_preference\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"policy_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"violations\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"opened_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-incident-response-type-schema.json
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
