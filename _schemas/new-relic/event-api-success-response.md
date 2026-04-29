---
description: Successful ingestion response
layout: schema
name: SuccessResponse
properties_list:
- description: Whether the request was accepted
  name: success
  type: boolean
- description: Unique request identifier
  name: uuid
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/event-api-success-response-schema.json
slug: event-api-success-response
source_filename: event-api-success-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-success-response-schema.json\",\n  \"title\": \"SuccessResponse\",\n  \"description\": \"Successful ingestion response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request was accepted\",\n      \"example\": true\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request identifier\",\n      \"example\": \"500123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-success-response-schema.json
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
title: SuccessResponse
---
