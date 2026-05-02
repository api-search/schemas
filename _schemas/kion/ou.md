---
description: An organizational unit (OU) provides hierarchical organization of projects, accounts, and governance policies in Kion.
layout: schema
name: Kion Organizational Unit
properties_list:
- description: Internal Kion OU ID.
  name: id
  type: integer
- description: OU name.
  name: name
  type: string
- description: OU description.
  name: description
  type: string
- description: Parent organizational unit ID.
  name: parent_ou_id
  type: integer
- description: Permission scheme ID applied to the OU.
  name: permission_scheme_id
  type: integer
- description: Labels associated with the OU.
  name: labels
  type: object
- description: Timestamp when the OU was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/ou.json
slug: ou
source_filename: ou.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/ou.json\",\n  \"title\": \"Kion Organizational Unit\",\n  \"description\": \"An organizational unit (OU) provides hierarchical organization of projects, accounts, and governance policies in Kion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion OU ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"OU name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"OU description.\"\n    },\n    \"parent_ou_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent organizational unit ID.\"\n    },\n    \"permission_scheme_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Permission scheme ID applied to the OU.\"\n    },\n    \"labels\": {\n      \"type\": \"object\"\
  ,\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the OU.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the OU was created.\"\n    }\n  },\n  \"required\": [\"name\", \"parent_ou_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/ou.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Organizational Unit
---
