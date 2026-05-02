---
description: A webhook provides event-driven notifications from Kion to external systems when cloud operations events occur.
layout: schema
name: Kion Webhook
properties_list:
- description: Internal Kion webhook ID.
  name: id
  type: integer
- description: Webhook name.
  name: name
  type: string
- description: Webhook description.
  name: description
  type: string
- description: Webhook destination URL.
  name: url
  type: string
- description: Authentication type for the webhook.
  name: auth_type
  type: string
- description: Authentication token for the webhook.
  name: auth_token
  type: string
- description: Owner users of the webhook.
  name: owner_users
  type: array
- description: Owner user groups of the webhook.
  name: owner_user_groups
  type: array
- description: Labels associated with the webhook.
  name: labels
  type: object
- description: Timestamp when the webhook was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/webhook.json
slug: webhook
source_filename: webhook.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/webhook.json\",\n  \"title\": \"Kion Webhook\",\n  \"description\": \"A webhook provides event-driven notifications from Kion to external systems when cloud operations events occur.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion webhook ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook description.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook destination URL.\"\n    },\n    \"auth_type\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type for the webhook.\"\n    },\n    \"auth_token\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Authentication token for the webhook.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the webhook.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the webhook.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the webhook.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the webhook was created.\"\n    }\n  },\n  \"required\": [\"name\"\
  , \"url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/webhook.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Webhook
---
