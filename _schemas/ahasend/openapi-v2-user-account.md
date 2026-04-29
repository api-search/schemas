---
description: UserAccount schema from AhaSend API
layout: schema
name: UserAccount
properties_list:
- description: Unique identifier for the user account relationship
  name: id
  type: string
- description: When the relationship was created
  name: created_at
  type: string
- description: When the relationship was last updated
  name: updated_at
  type: string
- description: User ID
  name: user_id
  type: string
- description: Account ID
  name: account_id
  type: string
- description: User role in the account
  name: role
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-user-account-schema.json
slug: openapi-v2-user-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-user-account-schema.json\",\n  \"title\": \"UserAccount\",\n  \"description\": \"UserAccount schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the user account relationship\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the relationship was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the relationship was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"user_id\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uuid\",\n      \"description\": \"User ID\",\n      \"example\": \"500123\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Account ID\",\n      \"example\": \"500123\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Administrator\",\n        \"Developer\",\n        \"Analyst\",\n        \"Billing Manager\"\n      ],\n      \"description\": \"User role in the account\",\n      \"example\": \"Administrator\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"user_id\",\n    \"account_id\",\n    \"role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-user-account-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: UserAccount
---
