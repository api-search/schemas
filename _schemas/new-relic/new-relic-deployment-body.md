---
description: ''
layout: schema
name: DeploymentBody
properties_list:
- description: ''
  name: changelog
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: revision
  type: string
- description: ''
  name: user
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-deployment-body-schema.json
slug: new-relic-deployment-body
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"changelog\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-deployment-body-schema.json
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
title: DeploymentBody
---
