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
schema_file: json-schema/new-relic-log-accepted-response-schema.json
slug: new-relic-log-accepted-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response when the payload was accepted\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the accepted ingestion request\",\n      \"example\": \"500123\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AcceptedResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-log-accepted-response-schema.json
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
