---
description: A cloud account managed by Kion across AWS, Azure, GCP, or OCI, linked to a project and payer for governance and cost tracking.
layout: schema
name: Kion Account
properties_list:
- description: Internal Kion account ID.
  name: id
  type: integer
- description: Account name.
  name: name
  type: string
- description: Cloud provider account number or ID.
  name: account_number
  type: string
- description: Account type identifier.
  name: account_type_id
  type: integer
- description: Payer account ID.
  name: payer_id
  type: integer
- description: Project ID the account belongs to.
  name: project_id
  type: integer
- description: Email associated with the account.
  name: email
  type: string
- description: Linked account number.
  name: linked_account_number
  type: string
- description: IAM role used for linked access.
  name: linked_role
  type: string
- description: Start date for the account.
  name: start_datecode
  type: string
- description: Whether to skip access checking.
  name: skip_access_checking
  type: boolean
- description: Whether to use organization account access role.
  name: use_org_account_access_role
  type: boolean
- description: Labels associated with the account.
  name: labels
  type: object
- description: Timestamp when the account was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/account.json
slug: account
source_filename: account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/account.json\",\n  \"title\": \"Kion Account\",\n  \"description\": \"A cloud account managed by Kion across AWS, Azure, GCP, or OCI, linked to a project and payer for governance and cost tracking.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion account ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name.\"\n    },\n    \"account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider account number or ID.\"\n    },\n    \"account_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Account type identifier.\"\n    },\n    \"payer_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Payer account ID.\"\n    },\n    \"project_id\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"Project ID the account belongs to.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email associated with the account.\"\n    },\n    \"linked_account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Linked account number.\"\n    },\n    \"linked_role\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role used for linked access.\"\n    },\n    \"start_datecode\": {\n      \"type\": \"string\",\n      \"description\": \"Start date for the account.\"\n    },\n    \"skip_access_checking\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to skip access checking.\"\n    },\n    \"use_org_account_access_role\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use organization account access role.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"\
  Labels associated with the account.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the account was created.\"\n    }\n  },\n  \"required\": [\"name\", \"account_number\", \"account_type_id\", \"payer_id\", \"project_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/account.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Account
---
