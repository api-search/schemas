---
description: A funding source represents a budget allocation for tracking and managing cloud spend within an organizational unit.
layout: schema
name: Kion Funding Source
properties_list:
- description: Internal Kion funding source ID.
  name: id
  type: integer
- description: Funding source name.
  name: name
  type: string
- description: Funding source description.
  name: description
  type: string
- description: Total funding amount.
  name: amount
  type: number
- description: Funding start date.
  name: start_datecode
  type: string
- description: Funding end date.
  name: end_datecode
  type: string
- description: Organizational unit ID the funding source belongs to.
  name: ou_id
  type: integer
- description: Owner users of the funding source.
  name: owner_users
  type: array
- description: Owner user groups of the funding source.
  name: owner_user_groups
  type: array
- description: Labels associated with the funding source.
  name: labels
  type: object
- description: Timestamp when the funding source was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/funding-source.json
slug: funding-source
source_filename: funding-source.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/funding-source.json\",\n  \"title\": \"Kion Funding Source\",\n  \"description\": \"A funding source represents a budget allocation for tracking and managing cloud spend within an organizational unit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion funding source ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Funding source name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Funding source description.\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total funding amount.\"\n    },\n    \"start_datecode\": {\n      \"type\": \"string\",\n      \"description\": \"Funding start date.\"\n    },\n    \"end_datecode\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Funding end date.\"\n    },\n    \"ou_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organizational unit ID the funding source belongs to.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the funding source.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the funding source.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the funding source.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the funding source was created.\"\n    }\n  },\n  \"required\": [\"name\", \"amount\", \"start_datecode\", \"end_datecode\", \"ou_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/funding-source.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Funding Source
---
