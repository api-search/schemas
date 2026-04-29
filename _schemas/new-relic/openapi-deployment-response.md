---
description: DeploymentResponse schema
layout: schema
name: DeploymentResponse
properties_list:
- description: ''
  name: deployment
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-deployment-response-schema.json
slug: openapi-deployment-response
source_filename: openapi-deployment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-response-schema.json\",\n  \"title\": \"DeploymentResponse\",\n  \"description\": \"DeploymentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment\": {\n      \"$ref\": \"#/components/schemas/DeploymentResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-deployment-response-schema.json
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
