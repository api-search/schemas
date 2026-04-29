---
description: An integration configuration for a linked account within the Cobalt embedded integration platform.
layout: schema
name: Config
properties_list:
- description: Configuration ID.
  name: _id
  type: string
- description: Application slug.
  name: slug
  type: string
- description: The linked account ID.
  name: linked_account_id
  type: string
- description: Configuration fields.
  name: fields
  type: object
- description: Workflow enablement settings.
  name: workflows
  type: array
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/config.json
slug: config
source_filename: config.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/config.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Config\",\n  \"description\": \"An integration configuration for a linked account within the Cobalt embedded integration platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration ID.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Application slug.\"\n    },\n    \"linked_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The linked account ID.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration fields.\"\n    },\n    \"workflows\": {\n      \"type\": \"array\",\n      \"description\": \"Workflow enablement settings.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"id\": {\n            \"type\": \"string\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/config.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Config
---
