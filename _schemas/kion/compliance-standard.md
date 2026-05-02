---
description: A compliance standard groups multiple compliance checks together to represent an industry or organizational compliance framework.
layout: schema
name: Kion Compliance Standard
properties_list:
- description: Internal Kion compliance standard ID.
  name: id
  type: integer
- description: Compliance standard name.
  name: name
  type: string
- description: Compliance standard description.
  name: description
  type: string
- description: Compliance check IDs included in this standard.
  name: compliance_checks
  type: array
- description: Owner users of the compliance standard.
  name: owner_users
  type: array
- description: Owner user groups of the compliance standard.
  name: owner_user_groups
  type: array
- description: Labels associated with the compliance standard.
  name: labels
  type: object
- description: Timestamp when the compliance standard was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/compliance-standard.json
slug: compliance-standard
source_filename: compliance-standard.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/compliance-standard.json\",\n  \"title\": \"Kion Compliance Standard\",\n  \"description\": \"A compliance standard groups multiple compliance checks together to represent an industry or organizational compliance framework.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion compliance standard ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance standard name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance standard description.\"\n    },\n    \"compliance_checks\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Compliance check IDs included in this standard.\"\n    },\n    \"owner_users\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the compliance standard.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the compliance standard.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the compliance standard.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the compliance standard was created.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/compliance-standard.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Compliance Standard
---
