---
description: Represents a 1Password vault that contains items. Vaults are used to organize and control access to secrets.
layout: schema
name: Vault
properties_list:
- description: The unique identifier for the vault.
  name: id
  type: string
- description: The name of the vault.
  name: name
  type: string
- description: A description of the vault's purpose.
  name: description
  type: string
- description: The version of the vault attributes.
  name: attributeVersion
  type: integer
- description: The version of the vault contents.
  name: contentVersion
  type: integer
- description: The number of items in the vault.
  name: items
  type: integer
- description: The type of the vault.
  name: type
  type: string
- description: The date and time the vault was created.
  name: createdAt
  type: string
- description: The date and time the vault was last updated.
  name: updatedAt
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-vault-schema.json
slug: 1password-connect-vault
source_filename: 1password-connect-vault-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-vault-schema.json\",\n  \"title\": \"Vault\",\n  \"description\": \"Represents a 1Password vault that contains items. Vaults are used to organize and control access to secrets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the vault.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the vault.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the vault's purpose.\"\n    },\n    \"attributeVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the vault attributes.\"\n    },\n    \"contentVersion\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"The version of the vault contents.\"\n    },\n    \"items\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the vault.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the vault.\",\n      \"enum\": [\n        \"USER_CREATED\",\n        \"PERSONAL\",\n        \"EVERYONE\",\n        \"TRANSFER\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the vault was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the vault was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-vault-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Vault
---
