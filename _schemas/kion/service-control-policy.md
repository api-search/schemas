---
description: An AWS service control policy (SCP) managed through Kion for restricting permissions across accounts in an AWS Organization.
layout: schema
name: Kion Service Control Policy
properties_list:
- description: Internal Kion SCP ID.
  name: id
  type: integer
- description: SCP name.
  name: name
  type: string
- description: SCP description.
  name: description
  type: string
- description: JSON policy document.
  name: policy
  type: string
- description: Owner users of the SCP.
  name: owner_users
  type: array
- description: Owner user groups of the SCP.
  name: owner_user_groups
  type: array
- description: Labels associated with the SCP.
  name: labels
  type: object
- description: Timestamp when the SCP was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/service-control-policy.json
slug: service-control-policy
source_filename: service-control-policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/service-control-policy.json\",\n  \"title\": \"Kion Service Control Policy\",\n  \"description\": \"An AWS service control policy (SCP) managed through Kion for restricting permissions across accounts in an AWS Organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion SCP ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"SCP name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"SCP description.\"\n    },\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"JSON policy document.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"\
  integer\" }\n        }\n      },\n      \"description\": \"Owner users of the SCP.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the SCP.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the SCP.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the SCP was created.\"\n    }\n  },\n  \"required\": [\"name\", \"policy\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/service-control-policy.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Service Control Policy
---
