---
description: A user group organizes users for role-based access control and permission management in Kion.
layout: schema
name: Kion User Group
properties_list:
- description: Internal Kion user group ID.
  name: id
  type: integer
- description: User group name.
  name: name
  type: string
- description: User group description.
  name: description
  type: string
- description: Identity management system ID.
  name: idms_id
  type: integer
- description: Users belonging to this group.
  name: users
  type: array
- description: Whether the user group is enabled.
  name: enabled
  type: boolean
- description: Timestamp when the user group was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/user-group.json
slug: user-group
source_filename: user-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/user-group.json\",\n  \"title\": \"Kion User Group\",\n  \"description\": \"A user group organizes users for role-based access control and permission management in Kion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion user group ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User group name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User group description.\"\n    },\n    \"idms_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identity management system ID.\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n     \
  \ },\n      \"description\": \"Users belonging to this group.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user group is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user group was created.\"\n    }\n  },\n  \"required\": [\"name\", \"idms_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/user-group.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion User Group
---
