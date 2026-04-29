---
description: Represents a summary of a 1Password item with basic metadata. Use the get item endpoint to retrieve full details.
layout: schema
name: Item
properties_list:
- description: The unique identifier for the item.
  name: id
  type: string
- description: The title of the item.
  name: title
  type: string
- description: ''
  name: vault
  type: object
- description: The category of the item.
  name: category
  type: string
- description: URLs associated with the item.
  name: urls
  type: array
- description: Whether the item is marked as a favorite.
  name: favorite
  type: boolean
- description: Tags applied to the item.
  name: tags
  type: array
- description: The version number of the item.
  name: version
  type: integer
- description: The state of the item.
  name: state
  type: string
- description: The date and time the item was created.
  name: createdAt
  type: string
- description: The date and time the item was last updated.
  name: updatedAt
  type: string
- description: The UUID of the user who last edited the item.
  name: lastEditedBy
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-item-schema.json
slug: 1password-connect-item
source_filename: 1password-connect-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-item-schema.json\",\n  \"title\": \"Item\",\n  \"description\": \"Represents a summary of a 1Password item with basic metadata. Use the get item endpoint to retrieve full details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the item.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the item.\"\n    },\n    \"vault\": {\n      \"$ref\": \"#/components/schemas/VaultRef\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the item.\",\n      \"enum\": [\n        \"LOGIN\",\n        \"PASSWORD\",\n        \"API_CREDENTIAL\",\n        \"SERVER\",\n        \"DATABASE\",\n  \
  \      \"CREDIT_CARD\",\n        \"MEMBERSHIP\",\n        \"PASSPORT\",\n        \"SOFTWARE_LICENSE\",\n        \"OUTDOOR_LICENSE\",\n        \"SECURE_NOTE\",\n        \"WIRELESS_ROUTER\",\n        \"BANK_ACCOUNT\",\n        \"DRIVER_LICENSE\",\n        \"IDENTITY\",\n        \"REWARD_PROGRAM\",\n        \"DOCUMENT\",\n        \"EMAIL_ACCOUNT\",\n        \"SOCIAL_SECURITY_NUMBER\",\n        \"MEDICAL_RECORD\",\n        \"SSH_KEY\",\n        \"CUSTOM\"\n      ]\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\": \"URLs associated with the item.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Url\"\n      }\n    },\n    \"favorite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the item is marked as a favorite.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the item.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"version\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The version number of the item.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the item.\",\n      \"enum\": [\n        \"ARCHIVED\",\n        \"DELETED\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item was last updated.\"\n    },\n    \"lastEditedBy\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the user who last edited the item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-item-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Item
---
