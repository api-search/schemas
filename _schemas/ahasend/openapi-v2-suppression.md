---
description: Suppression schema from AhaSend API
layout: schema
name: Suppression
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the suppression
  name: id
  type: string
- description: When the suppression was created
  name: created_at
  type: string
- description: When the suppression was last updated
  name: updated_at
  type: string
- description: Suppressed email address
  name: email
  type: string
- description: Domain for which the email is suppressed
  name: domain
  type: string
- description: Reason for suppression
  name: reason
  type: string
- description: When the suppression expires
  name: expires_at
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-suppression-schema.json
slug: openapi-v2-suppression
source_filename: openapi-v2-suppression-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-suppression-schema.json\",\n  \"title\": \"Suppression\",\n  \"description\": \"Suppression schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"suppression\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"suppression\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the suppression\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the suppression was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"When the suppression was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Suppressed email address\",\n      \"example\": \"user@example.com\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Domain for which the email is suppressed\",\n      \"example\": \"mail.example.com\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Reason for suppression\",\n      \"example\": \"example_value\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the suppression expires\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"email\",\n    \"\
  expires_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-suppression-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Suppression
---
