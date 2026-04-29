---
description: NrqlConditionResponse schema
layout: schema
name: NrqlConditionResponse
properties_list:
- description: ''
  name: nrql_condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-nrql-condition-response-schema.json
slug: openapi-nrql-condition-response
source_filename: openapi-nrql-condition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-response-schema.json\",\n  \"title\": \"NrqlConditionResponse\",\n  \"description\": \"NrqlConditionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nrql_condition\": {\n      \"$ref\": \"#/components/schemas/NrqlConditionResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-response-schema.json
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
title: NrqlConditionResponse
---
