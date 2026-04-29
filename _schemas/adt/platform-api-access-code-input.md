---
description: Request to create an access code.
layout: schema
name: AccessCodeInput
properties_list:
- description: Display name for the access code.
  name: name
  type: string
- description: The numeric access code (4-8 digits).
  name: code
  type: string
- description: Type of access code.
  name: type
  type: string
- description: Expiration time for temporary codes.
  name: expiresAt
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-access-code-input-schema.json
slug: platform-api-access-code-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-input-schema.json\",\n  \"title\": \"AccessCodeInput\",\n  \"description\": \"Request to create an access code.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"code\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the access code.\",\n      \"example\": \"Contractor Code\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The numeric access code (4-8 digits).\",\n      \"example\": \"5678\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of access code.\",\n      \"enum\": [\n        \"standard\",\n        \"temporary\"\n      ],\n      \"example\": \"temporary\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Expiration time for temporary codes.\",\n      \"example\": \"2025-03-20T23:59:59Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-input-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: AccessCodeInput
---
