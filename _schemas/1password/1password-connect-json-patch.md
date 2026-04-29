---
description: A JSON Patch document as defined by RFC 6902 for applying partial modifications to items.
layout: schema
name: JsonPatch
properties_list: []
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-json-patch-schema.json
slug: 1password-connect-json-patch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-json-patch-schema.json\",\n  \"title\": \"JsonPatch\",\n  \"description\": \"A JSON Patch document as defined by RFC 6902 for applying partial modifications to items.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"op\",\n      \"path\"\n    ],\n    \"properties\": {\n      \"op\": {\n        \"type\": \"string\",\n        \"description\": \"The operation to perform.\",\n        \"enum\": [\n          \"add\",\n          \"remove\",\n          \"replace\"\n        ]\n      },\n      \"path\": {\n        \"type\": \"string\",\n        \"description\": \"A JSON Pointer to the target location in the item.\"\n      },\n      \"value\": {\n        \"description\": \"The value to use in the operation. Required for add and replace.\"\n      }\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-json-patch-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: JsonPatch
---
