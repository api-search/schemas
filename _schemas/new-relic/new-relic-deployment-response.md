---
description: ''
layout: schema
name: DeploymentResponse
properties_list:
- description: ''
  name: deployment
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-deployment-response-schema.json
slug: new-relic-deployment-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"changelog\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"application\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            }\n          }\n        },\n        \"revision\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2026-04-18T14:30:00Z\"\n        },\n        \"user\": {\n          \"type\": \"\
  string\",\n          \"example\": \"example_string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-deployment-response-schema.json
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
title: DeploymentResponse
---
