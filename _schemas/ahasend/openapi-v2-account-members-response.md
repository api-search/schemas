---
description: AccountMembersResponse schema from AhaSend API
layout: schema
name: AccountMembersResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Array of account members
  name: data
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-account-members-response-schema.json
slug: openapi-v2-account-members-response
source_filename: openapi-v2-account-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-account-members-response-schema.json\",\n  \"title\": \"AccountMembersResponse\",\n  \"description\": \"AccountMembersResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserAccount\"\n      },\n      \"description\": \"Array of account members\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"created_at\": \"2025-03-15T14:30:00Z\",\n          \"updated_at\": \"2025-03-15T14:30:00Z\",\n          \"user_id\": \"500123\",\n          \"account_id\": \"500123\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-account-members-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: AccountMembersResponse
---
