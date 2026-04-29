---
description: Application schema
layout: schema
name: Application
properties_list:
- description: ''
  name: application
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-schema.json
slug: openapi-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"Application schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"$ref\": \"#/components/schemas/ApplicationBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-schema.json
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
title: Application
---
