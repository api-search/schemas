---
description: ''
layout: schema
name: Policy
properties_list:
- description: ''
  name: policy
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-policy-schema.json
slug: new-relic-policy
source_filename: new-relic-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"incident_preference\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Policy\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-policy-schema.json
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
title: Policy
---
