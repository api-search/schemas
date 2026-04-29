---
description: CreateSuppressionRequest schema from AhaSend API
layout: schema
name: CreateSuppressionRequest
properties_list:
- description: Email address to suppress
  name: email
  type: string
- description: Domain for which to suppress the email
  name: domain
  type: string
- description: Reason for suppression
  name: reason
  type: string
- description: When the suppression expires (RFC3339 format)
  name: expires_at
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-suppression-request-schema.json
slug: openapi-v2-create-suppression-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-suppression-request-schema.json\",\n  \"title\": \"CreateSuppressionRequest\",\n  \"description\": \"CreateSuppressionRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address to suppress\",\n      \"example\": \"user@example.com\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"format\": \"hostname\",\n      \"description\": \"Domain for which to suppress the email\",\n      \"example\": \"mail.example.com\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Reason for suppression\",\n      \"example\": \"example_value\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"When the suppression expires (RFC3339 format)\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"expires_at\"\n  ],\n  \"example\": {\n    \"email\": \"user@example.com\",\n    \"domain\": \"example.com\",\n    \"reason\": \"User requested removal\",\n    \"expires_at\": \"2024-12-25T10:30:00Z\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-suppression-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateSuppressionRequest
---
