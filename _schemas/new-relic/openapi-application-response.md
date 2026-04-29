---
description: ApplicationResponse schema
layout: schema
name: ApplicationResponse
properties_list:
- description: ''
  name: application
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-response-schema.json
slug: openapi-application-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-response-schema.json\",\n  \"title\": \"ApplicationResponse\",\n  \"description\": \"ApplicationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"$ref\": \"#/components/schemas/ApplicationResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-response-schema.json
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
title: ApplicationResponse
---
