---
description: PolicyResponse schema
layout: schema
name: PolicyResponse
properties_list:
- description: ''
  name: policy
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-policy-response-schema.json
slug: openapi-policy-response
source_filename: openapi-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-response-schema.json\",\n  \"title\": \"PolicyResponse\",\n  \"description\": \"PolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"$ref\": \"#/components/schemas/PolicyResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-response-schema.json
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
