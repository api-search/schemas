---
description: ''
layout: schema
name: HecResponse
properties_list:
- description: Human-readable status message
  name: text
  type: string
- description: Numeric status code
  name: code
  type: integer
- description: For batched events, the index of the first invalid event
  name: invalid-event-number
  type: integer
- description: Acknowledgment ID for tracking indexing status (when indexer acknowledgment is enabled)
  name: ackId
  type: integer
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-hec-response-schema.json
slug: splunk-enterprise-rest-hec-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HecResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status message\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric status code\"\n    },\n    \"invalid-event-number\": {\n      \"type\": \"integer\",\n      \"description\": \"For batched events, the index of the first invalid event\"\n    },\n    \"ackId\": {\n      \"type\": \"integer\",\n      \"description\": \"Acknowledgment ID for tracking indexing status (when indexer acknowledgment is enabled)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-hec-response-schema.json
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
title: HecResponse
---
