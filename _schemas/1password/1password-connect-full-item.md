---
description: Represents a complete 1Password item including all fields, sections, and associated metadata. Used for creating and updating items.
layout: schema
name: FullItem
properties_list: []
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-full-item-schema.json
slug: 1password-connect-full-item
source_filename: 1password-connect-full-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-full-item-schema.json\",\n  \"title\": \"FullItem\",\n  \"description\": \"Represents a complete 1Password item including all fields, sections, and associated metadata. Used for creating and updating items.\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Item\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fields\": {\n          \"type\": \"array\",\n          \"description\": \"The fields of the item containing secrets and metadata.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Field\"\n          }\n        },\n        \"sections\": {\n          \"type\": \"array\",\n          \"description\": \"Sections used to organize fields within the item.\",\n          \"items\": {\n            \"\
  $ref\": \"#/components/schemas/Section\"\n          }\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-full-item-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: FullItem
---
