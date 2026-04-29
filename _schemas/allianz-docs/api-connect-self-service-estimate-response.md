---
description: Self-service estimate session with redirect URL for customer
layout: schema
name: SelfServiceEstimateResponse
properties_list:
- description: Unique identifier for the estimate session
  name: session_id
  type: string
- description: URL for the customer to view and complete their estimate
  name: estimate_url
  type: string
- description: Timestamp when the session expires
  name: expires_at
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-self-service-estimate-response-schema.json
slug: api-connect-self-service-estimate-response
source_filename: api-connect-self-service-estimate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-self-service-estimate-response-schema.json\",\n  \"title\": \"SelfServiceEstimateResponse\",\n  \"description\": \"Self-service estimate session with redirect URL for customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the estimate session\",\n      \"example\": \"ses-500789\"\n    },\n    \"estimate_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the customer to view and complete their estimate\",\n      \"example\": \"https://quote.allianz.com.au/session/ses-500789\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the session expires\",\n      \"example\"\
  : \"2026-04-19T22:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-self-service-estimate-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: SelfServiceEstimateResponse
---
