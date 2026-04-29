---
description: ''
layout: schema
name: Deployment
properties_list:
- description: ''
  name: deployment
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-deployment-schema.json
slug: new-relic-deployment
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"changelog\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"revision\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-deployment-schema.json
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
title: Deployment
---
