---
description: ''
layout: schema
name: ViolationLinksResponse
properties_list:
- description: ''
  name: condition_id
  type: integer
- description: ''
  name: incident_id
  type: integer
- description: ''
  name: policy_id
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-violation-links-response-schema.json
slug: new-relic-violation-links-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"incident_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"policy_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViolationLinksResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-violation-links-response-schema.json
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
title: ViolationLinksResponse
---
