---
description: A custom variable stores key-value configuration data that can be referenced across cloud rules, templates, and other Kion resources, with optional OU and project-level overrides.
layout: schema
name: Kion Custom Variable
properties_list:
- description: Internal Kion custom variable ID.
  name: id
  type: integer
- description: Variable key.
  name: key
  type: string
- description: Variable value.
  name: value
  type: string
- description: Variable description.
  name: description
  type: string
- description: Labels associated with the variable.
  name: labels
  type: object
- description: Timestamp when the variable was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/custom-variable.json
slug: custom-variable
source_filename: custom-variable.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/custom-variable.json\",\n  \"title\": \"Kion Custom Variable\",\n  \"description\": \"A custom variable stores key-value configuration data that can be referenced across cloud rules, templates, and other Kion resources, with optional OU and project-level overrides.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion custom variable ID.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Variable key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Variable value.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Variable description.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      },\n      \"description\": \"Labels associated with the variable.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the variable was created.\"\n    }\n  },\n  \"required\": [\"key\", \"value\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/custom-variable.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Custom Variable
---
