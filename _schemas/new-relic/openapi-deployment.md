---
description: Deployment schema
layout: schema
name: Deployment
properties_list:
- description: ''
  name: deployment
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-deployment-schema.json
slug: openapi-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-schema.json\",\n  \"title\": \"Deployment\",\n  \"description\": \"Deployment schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment\": {\n      \"$ref\": \"#/components/schemas/DeploymentBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-schema.json
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
