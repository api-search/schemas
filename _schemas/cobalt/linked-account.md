---
description: A linked account representing an end-customer within the Cobalt embedded integration platform.
layout: schema
name: LinkedAccount
properties_list:
- description: Internal identifier.
  name: _id
  type: string
- description: The unique identifier for the linked account.
  name: linked_account_id
  type: string
- description: Display name.
  name: name
  type: string
- description: Custom metadata.
  name: your_app
  type: object
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/linked-account.json
slug: linked-account
source_filename: linked-account.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/linked-account.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinkedAccount\",\n  \"description\": \"A linked account representing an end-customer within the Cobalt embedded integration platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal identifier.\"\n    },\n    \"linked_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the linked account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name.\"\n    },\n    \"your_app\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    },\n    \"updated_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/linked-account.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: LinkedAccount
---
