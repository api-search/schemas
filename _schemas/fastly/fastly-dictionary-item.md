---
description: A single key-value pair within a Fastly edge dictionary. Dictionary items are versionless and can be updated without requiring a new service version. Updates are available at the edge within approximately 30 seconds.
layout: schema
name: Fastly Dictionary Item
properties_list:
- description: The alphanumeric string identifying the parent dictionary.
  name: dictionary_id
  type: string
- description: The alphanumeric string identifying the service.
  name: service_id
  type: string
- description: The key of the dictionary item.
  name: item_key
  type: string
- description: The value of the dictionary item.
  name: item_value
  type: string
- description: The date and time the item was created.
  name: created_at
  type: string
- description: The date and time the item was last updated.
  name: updated_at
  type: string
- description: The date and time the item was deleted.
  name: deleted_at
  type:
  - string
  - 'null'
provider_name: fastly
provider_slug: fastly
schema_file: json-schema/fastly-dictionary-item-schema.json
slug: fastly-dictionary-item
source_filename: fastly-dictionary-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/fastly/dictionary-item.json\",\n  \"title\": \"Fastly Dictionary Item\",\n  \"description\": \"A single key-value pair within a Fastly edge dictionary. Dictionary items are versionless and can be updated without requiring a new service version. Updates are available at the edge within approximately 30 seconds.\",\n  \"type\": \"object\",\n  \"required\": [\"item_key\", \"item_value\"],\n  \"properties\": {\n    \"dictionary_id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the parent dictionary.\"\n    },\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the service.\"\n    },\n    \"item_key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the dictionary item.\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n  \
  \  \"item_value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the dictionary item.\",\n      \"maxLength\": 8000\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item was last updated.\"\n    },\n    \"deleted_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item was deleted.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/json-schema/fastly-dictionary-item-schema.json
tags: []
title: Fastly Dictionary Item
---
