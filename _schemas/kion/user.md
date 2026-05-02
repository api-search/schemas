---
description: A user within the Kion platform, associated with an identity management system for authentication and access control.
layout: schema
name: Kion User
properties_list:
- description: Internal Kion user ID.
  name: id
  type: integer
- description: Username for authentication.
  name: username
  type: string
- description: User first name.
  name: first_name
  type: string
- description: User last name.
  name: last_name
  type: string
- description: User email address.
  name: email
  type: string
- description: Identity management system ID.
  name: idms_id
  type: integer
- description: Whether the user account is enabled.
  name: enabled
  type: boolean
- description: Timestamp when the user was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/user.json\",\n  \"title\": \"Kion User\",\n  \"description\": \"A user within the Kion platform, associated with an identity management system for authentication and access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion user ID.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username for authentication.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"User first name.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"User last name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"User email address.\"\n    },\n    \"idms_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identity\
  \ management system ID.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was created.\"\n    }\n  },\n  \"required\": [\"username\", \"first_name\", \"last_name\", \"email\", \"idms_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/user.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion User
---
