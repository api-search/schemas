---
description: NrqlCondition schema
layout: schema
name: NrqlCondition
properties_list:
- description: ''
  name: nrql_condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-nrql-condition-schema.json
slug: openapi-nrql-condition
source_filename: openapi-nrql-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-schema.json\",\n  \"title\": \"NrqlCondition\",\n  \"description\": \"NrqlCondition schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nrql_condition\": {\n      \"$ref\": \"#/components/schemas/NrqlConditionBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-nrql-condition-schema.json
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
title: NrqlCondition
---
