---
description: An Airgas B2B customer account.
layout: schema
name: Account
properties_list:
- description: Unique Airgas account number.
  name: account_number
  type: string
- description: Business name for the account.
  name: company_name
  type: string
- description: Type of customer account.
  name: account_type
  type: string
- description: ''
  name: primary_contact
  type: object
- description: ''
  name: billing_address
  type: object
- description: Account credit limit in USD.
  name: credit_limit
  type: number
- description: Payment terms for the account.
  name: payment_terms
  type: string
- description: Whether the account is active.
  name: is_active
  type: boolean
provider_name: Airgas
provider_slug: airgas
schema_file: json-schema/airgas-account-schema.json
slug: airgas-account
source_filename: airgas-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"An Airgas B2B customer account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Airgas account number.\",\n      \"example\": \"ACCT-789012\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Business name for the account.\",\n      \"example\": \"Precision Metal Works Inc.\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"industrial\", \"medical\", \"food\", \"retail\", \"government\"],\n      \"description\": \"Type of customer account.\",\n      \"example\": \"industrial\"\n    },\n    \"primary_contact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"\
  name\": {\"type\": \"string\", \"example\": \"Jane Smith\"},\n        \"email\": {\"type\": \"string\", \"format\": \"email\", \"example\": \"jane.smith@example.com\"},\n        \"phone\": {\"type\": \"string\", \"example\": \"+1-713-555-0100\"}\n      }\n    },\n    \"billing_address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"string\"},\n        \"state\": {\"type\": \"string\"},\n        \"zip\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\"}\n      }\n    },\n    \"credit_limit\": {\n      \"type\": \"number\",\n      \"description\": \"Account credit limit in USD.\",\n      \"example\": 50000.00\n    },\n    \"payment_terms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms for the account.\",\n      \"example\": \"NET30\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is active.\",\n   \
  \   \"example\": true\n    }\n  },\n  \"required\": [\"account_number\", \"company_name\", \"account_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-account-schema.json
tags:
- Industrial Gases
- Welding
- Safety
- B2B
- Supply Chain
- Manufacturing
- Healthcare
title: Account
---
