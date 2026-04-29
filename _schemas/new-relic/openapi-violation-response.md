---
description: ViolationResponse schema
layout: schema
name: ViolationResponse
properties_list:
- description: ''
  name: violation
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-violation-response-schema.json
slug: openapi-violation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-violation-response-schema.json\",\n  \"title\": \"ViolationResponse\",\n  \"description\": \"ViolationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"violation\": {\n      \"$ref\": \"#/components/schemas/ViolationResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-violation-response-schema.json
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
title: ViolationResponse
---
