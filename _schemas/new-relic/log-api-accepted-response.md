---
description: Response when the payload was accepted
layout: schema
name: AcceptedResponse
properties_list:
- description: Unique identifier for the accepted ingestion request
  name: requestId
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/log-api-accepted-response-schema.json
slug: log-api-accepted-response
source_filename: log-api-accepted-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-accepted-response-schema.json\",\n  \"title\": \"AcceptedResponse\",\n  \"description\": \"Response when the payload was accepted\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the accepted ingestion request\",\n      \"example\": \"500123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-accepted-response-schema.json
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
title: AcceptedResponse
---
