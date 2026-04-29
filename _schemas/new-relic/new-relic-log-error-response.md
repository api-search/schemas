---
description: Error response
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: error
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-log-error-response-schema.json
slug: new-relic-log-error-response
source_filename: new-relic-log-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"type\": \"standard\",\n        \"message\": \"Operation completed successfully\"\n      },\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"message\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-log-error-response-schema.json
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
title: ErrorResponse
---
