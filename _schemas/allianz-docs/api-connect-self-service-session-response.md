---
description: Self-service session URL for customer to complete policy details
layout: schema
name: SelfServiceSessionResponse
properties_list:
- description: Unique identifier for the self-service session
  name: session_id
  type: string
- description: URL for the customer to complete their policy application
  name: session_url
  type: string
- description: Timestamp when the session expires
  name: expires_at
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-self-service-session-response-schema.json
slug: api-connect-self-service-session-response
source_filename: api-connect-self-service-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-self-service-session-response-schema.json\",\n  \"title\": \"SelfServiceSessionResponse\",\n  \"description\": \"Self-service session URL for customer to complete policy details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the self-service session\",\n      \"example\": \"ses-500891\"\n    },\n    \"session_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the customer to complete their policy application\",\n      \"example\": \"https://apply.allianz.com.au/session/ses-500891\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the session expires\",\n      \"\
  example\": \"2026-04-19T22:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-self-service-session-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: SelfServiceSessionResponse
---
