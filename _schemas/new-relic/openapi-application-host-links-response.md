---
description: ApplicationHostLinksResponse schema
layout: schema
name: ApplicationHostLinksResponse
properties_list:
- description: ''
  name: application
  type: integer
- description: ''
  name: application_instances
  type: array
- description: ''
  name: server
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-host-links-response-schema.json
slug: openapi-application-host-links-response
source_filename: openapi-application-host-links-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-links-response-schema.json\",\n  \"title\": \"ApplicationHostLinksResponse\",\n  \"description\": \"ApplicationHostLinksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"application_instances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    },\n    \"server\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-links-response-schema.json
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
title: ApplicationHostLinksResponse
---
