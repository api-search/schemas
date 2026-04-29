---
description: A Managed Account representing a linked cloud provider account within Vantage.
layout: schema
name: Vantage Managed Account
properties_list:
- description: The unique token identifier for the Managed Account.
  name: token
  type: string
- description: The name of the Managed Account.
  name: name
  type: string
- description: The cloud provider account identifier.
  name: account_identifier
  type: string
- description: The cloud provider.
  name: provider
  type: string
- description: The date and time the Managed Account was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/managed-account.json
slug: managed-account
source_filename: managed-account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/managed-account.json\",\n  \"title\": \"Vantage Managed Account\",\n  \"description\": \"A Managed Account representing a linked cloud provider account within Vantage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Managed Account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Managed Account.\"\n    },\n    \"account_identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider account identifier.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the\
  \ Managed Account was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/managed-account.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Managed Account
---
