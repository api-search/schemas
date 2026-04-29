---
description: SMTPCredential schema from AhaSend API
layout: schema
name: SMTPCredential
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the SMTP credential
  name: id
  type: string
- description: When the credential was created
  name: created_at
  type: string
- description: When the credential was last updated
  name: updated_at
  type: string
- description: Credential name
  name: name
  type: string
- description: SMTP username
  name: username
  type: string
- description: Whether this is a sandbox credential
  name: sandbox
  type: boolean
- description: Credential scope
  name: scope
  type: string
- description: Domains this credential can send from
  name: domains
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-smtp-credential-schema.json
slug: openapi-v2-smtp-credential
source_filename: openapi-v2-smtp-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-smtp-credential-schema.json\",\n  \"title\": \"SMTPCredential\",\n  \"description\": \"SMTPCredential schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"smtp_credential\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"smtp_credential\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the SMTP credential\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the credential was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the credential was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Credential name\",\n      \"example\": \"Example Name\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"SMTP username\",\n      \"example\": \"Example Name\"\n    },\n    \"sandbox\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a sandbox credential\",\n      \"example\": true\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"global\",\n        \"scoped\"\n      ],\n      \"description\": \"Credential scope\",\n      \"example\": \"global\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Domains this credential can send from\",\n      \"example\": [\n        \"mail.example.com\"\
  \n      ]\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"name\",\n    \"username\",\n    \"sandbox\",\n    \"scope\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-smtp-credential-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: SMTPCredential
---
