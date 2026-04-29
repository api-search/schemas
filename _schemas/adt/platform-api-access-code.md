---
description: An access code for a security system.
layout: schema
name: AccessCode
properties_list:
- description: Unique identifier of the access code.
  name: id
  type: string
- description: Display name for the access code.
  name: name
  type: string
- description: Type of access code.
  name: type
  type: string
- description: Expiration timestamp for temporary codes.
  name: expiresAt
  type: string
- description: List of permissions granted by this code.
  name: permissions
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-access-code-schema.json
slug: platform-api-access-code
source_filename: platform-api-access-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-schema.json\",\n  \"title\": \"AccessCode\",\n  \"description\": \"An access code for a security system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the access code.\",\n      \"example\": \"code-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the access code.\",\n      \"example\": \"Master Code\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of access code.\",\n      \"enum\": [\n        \"master\",\n        \"standard\",\n        \"temporary\",\n        \"duress\"\n      ],\n      \"example\": \"standard\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n\
  \      \"description\": \"Expiration timestamp for temporary codes.\",\n      \"example\": \"2025-03-20T23:59:59Z\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"List of permissions granted by this code.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: AccessCode
---
