---
description: ''
layout: schema
name: PolicyResponse
properties_list:
- description: ''
  name: policy
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-policy-response-schema.json
slug: new-relic-policy-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"created_at\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"incident_preference\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"updated_at\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-policy-response-schema.json
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
title: PolicyResponse
---
