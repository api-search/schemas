---
description: ConditionResponse schema
layout: schema
name: ConditionResponse
properties_list:
- description: ''
  name: condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-condition-response-schema.json
slug: openapi-condition-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-condition-response-schema.json\",\n  \"title\": \"ConditionResponse\",\n  \"description\": \"ConditionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"$ref\": \"#/components/schemas/ConditionResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-condition-response-schema.json
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
title: ConditionResponse
---
