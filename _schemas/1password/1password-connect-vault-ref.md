---
description: A reference to a vault.
layout: schema
name: VaultRef
properties_list:
- description: The unique identifier of the referenced vault.
  name: id
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-vault-ref-schema.json
slug: 1password-connect-vault-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-vault-ref-schema.json\",\n  \"title\": \"VaultRef\",\n  \"description\": \"A reference to a vault.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the referenced vault.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-vault-ref-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: VaultRef
---
