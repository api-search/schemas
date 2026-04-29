---
description: An Airwallex cross-border transfer to a beneficiary account.
layout: schema
name: Transfer
properties_list:
- description: Unique transfer identifier.
  name: id
  type: string
- description: Amount debited from the source account.
  name: source_amount
  type: number
- description: ISO 4217 currency code of the source amount.
  name: source_currency
  type: string
- description: Amount received by the beneficiary.
  name: target_amount
  type: number
- description: ISO 4217 currency code of the target amount.
  name: target_currency
  type: string
- description: Current transfer status.
  name: status
  type: string
- description: ID of the beneficiary account.
  name: beneficiary_id
  type: string
- description: Payment reference for the transfer.
  name: reference
  type: string
- description: Transfer fee charged.
  name: fee
  type: number
- description: Currency of the fee.
  name: fee_currency
  type: string
- description: Applied foreign exchange rate.
  name: fx_rate
  type: number
- description: Timestamp when the transfer was created.
  name: created_at
  type: string
provider_name: Airwallex
provider_slug: airwallex
schema_file: json-schema/airwallex-transfer-schema.json
slug: airwallex-transfer
source_filename: airwallex-transfer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-transfer-schema.json\",\n  \"title\": \"Transfer\",\n  \"description\": \"An Airwallex cross-border transfer to a beneficiary account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transfer identifier.\",\n      \"example\": \"txf_abc123def456\"\n    },\n    \"source_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount debited from the source account.\",\n      \"example\": 1000.00\n    },\n    \"source_currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code of the source amount.\",\n      \"example\": \"USD\"\n    },\n    \"target_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount received by the beneficiary.\",\n      \"example\": 920.50\n\
  \    },\n    \"target_currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code of the target amount.\",\n      \"example\": \"EUR\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"CREATED\", \"PENDING\", \"SUBMITTED\", \"SETTLED\", \"FAILED\", \"CANCELLED\"],\n      \"description\": \"Current transfer status.\",\n      \"example\": \"SETTLED\"\n    },\n    \"beneficiary_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the beneficiary account.\",\n      \"example\": \"ben_abc123\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Payment reference for the transfer.\",\n      \"example\": \"Invoice-2026-001\"\n    },\n    \"fee\": {\n      \"type\": \"number\",\n      \"description\": \"Transfer fee charged.\",\n      \"example\": 5.00\n    },\n    \"fee_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the fee.\",\n      \"example\": \"USD\"\
  \n    },\n    \"fx_rate\": {\n      \"type\": \"number\",\n      \"description\": \"Applied foreign exchange rate.\",\n      \"example\": 0.9205\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transfer was created.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  },\n  \"required\": [\"id\", \"source_amount\", \"source_currency\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-transfer-schema.json
tags:
- Cross-Border Payments
- FinTech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
title: Transfer
---
