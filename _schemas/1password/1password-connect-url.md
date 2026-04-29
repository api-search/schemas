---
description: Represents a URL associated with an item.
layout: schema
name: Url
properties_list:
- description: Whether this is the primary URL for the item.
  name: primary
  type: boolean
- description: The URL value.
  name: href
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-url-schema.json
slug: 1password-connect-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-url-schema.json\",\n  \"title\": \"Url\",\n  \"description\": \"Represents a URL associated with an item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"primary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary URL for the item.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-url-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Url
---
