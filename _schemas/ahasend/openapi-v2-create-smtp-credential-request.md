---
description: CreateSMTPCredentialRequest schema from AhaSend API
layout: schema
name: CreateSMTPCredentialRequest
properties_list:
- description: Credential name
  name: name
  type: string
- description: Whether this is a sandbox credential
  name: sandbox
  type: boolean
- description: Credential scope - "global" or "scoped"
  name: scope
  type: string
- description: Required if scope is "scoped"
  name: domains
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-smtp-credential-request-schema.json
slug: openapi-v2-create-smtp-credential-request
source_filename: openapi-v2-create-smtp-credential-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-smtp-credential-request-schema.json\",\n  \"title\": \"CreateSMTPCredentialRequest\",\n  \"description\": \"CreateSMTPCredentialRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Credential name\",\n      \"example\": \"Example Name\"\n    },\n    \"sandbox\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a sandbox credential\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"global\",\n        \"scoped\"\n      ],\n      \"description\": \"Credential scope - \\\"global\\\" or \\\"scoped\\\"\",\n      \"example\": \"global\"\n    },\n    \"domains\":\
  \ {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Required if scope is \\\"scoped\\\"\",\n      \"example\": [\n        \"mail.example.com\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"scope\"\n  ],\n  \"example\": {\n    \"name\": \"Production SMTP\",\n    \"username\": \"smtp_user\",\n    \"password\": \"secure_password\",\n    \"scope\": \"global\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-smtp-credential-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateSMTPCredentialRequest
---
