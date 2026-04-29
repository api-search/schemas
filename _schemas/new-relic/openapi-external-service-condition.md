---
description: ExternalServiceCondition schema
layout: schema
name: ExternalServiceCondition
properties_list:
- description: ''
  name: external_service_condition
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-external-service-condition-schema.json
slug: openapi-external-service-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-external-service-condition-schema.json\",\n  \"title\": \"ExternalServiceCondition\",\n  \"description\": \"ExternalServiceCondition schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external_service_condition\": {\n      \"$ref\": \"#/components/schemas/ExternalServiceConditionBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-external-service-condition-schema.json
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
title: ExternalServiceCondition
---
