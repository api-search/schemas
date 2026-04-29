---
description: Represents a record of an item in a shared vault being accessed, modified, or used.
layout: schema
name: ItemUsage
properties_list:
- description: The unique identifier for the item usage record.
  name: uuid
  type: string
- description: When the item was accessed.
  name: timestamp
  type: string
- description: The version of the item that was used.
  name: used_version
  type: integer
- description: The UUID of the vault containing the item.
  name: vault_uuid
  type: string
- description: The UUID of the item that was used.
  name: item_uuid
  type: string
- description: The type of action performed on the item.
  name: action
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: client
  type: object
- description: ''
  name: location
  type: object
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-item-usage-schema.json
slug: 1password-events-item-usage
source_filename: 1password-events-item-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-item-usage-schema.json\",\n  \"title\": \"ItemUsage\",\n  \"description\": \"Represents a record of an item in a shared vault being accessed, modified, or used.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the item usage record.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the item was accessed.\"\n    },\n    \"used_version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the item that was used.\"\n    },\n    \"vault_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the vault containing the item.\"\n\
  \    },\n    \"item_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the item that was used.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The type of action performed on the item.\",\n      \"enum\": [\n        \"fill\",\n        \"copy\",\n        \"reveal\",\n        \"sso-fill\",\n        \"secure-copy\"\n      ]\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/EventUser\"\n    },\n    \"client\": {\n      \"$ref\": \"#/components/schemas/EventClient\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/EventLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-item-usage-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: ItemUsage
---
