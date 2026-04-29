---
description: An Airwallex global multi-currency account.
layout: schema
name: Account
properties_list:
- description: Unique account identifier.
  name: id
  type: string
- description: Business name of the account holder.
  name: account_name
  type: string
- description: Account status.
  name: status
  type: string
- description: Primary currency for the account.
  name: primary_currency
  type: string
- description: Currency balances held in the account.
  name: balances
  type: array
- description: ISO 3166-1 alpha-2 country code of the account.
  name: country_code
  type: string
- description: Account creation timestamp.
  name: created_at
  type: string
provider_name: Airwallex
provider_slug: airwallex
schema_file: json-schema/airwallex-account-schema.json
slug: airwallex-account
source_filename: airwallex-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"An Airwallex global multi-currency account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier.\",\n      \"example\": \"acct_abc123def456\"\n    },\n    \"account_name\": {\n      \"type\": \"string\",\n      \"description\": \"Business name of the account holder.\",\n      \"example\": \"ACME Corp Ltd\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"PENDING\", \"ACTIVE\", \"SUSPENDED\", \"CLOSED\"],\n      \"description\": \"Account status.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"primary_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Primary currency for the account.\",\n  \
  \    \"example\": \"USD\"\n    },\n    \"balances\": {\n      \"type\": \"array\",\n      \"description\": \"Currency balances held in the account.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"currency\": {\"type\": \"string\"},\n          \"available_amount\": {\"type\": \"number\"},\n          \"pending_amount\": {\"type\": \"number\"}\n        }\n      }\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code of the account.\",\n      \"example\": \"US\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp.\",\n      \"example\": \"2026-01-15T08:00:00Z\"\n    }\n  },\n  \"required\": [\"id\", \"account_name\", \"status\", \"primary_currency\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-account-schema.json
tags:
- Cross-Border Payments
- FinTech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
title: Account
---
