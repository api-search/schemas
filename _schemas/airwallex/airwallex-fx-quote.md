---
description: An Airwallex foreign exchange rate quote for currency conversion.
layout: schema
name: FxQuote
properties_list:
- description: Unique quote identifier.
  name: quote_id
  type: string
- description: Source currency ISO 4217 code.
  name: from_currency
  type: string
- description: Target currency ISO 4217 code.
  name: to_currency
  type: string
- description: Quoted exchange rate (from_currency to to_currency).
  name: rate
  type: number
- description: Source amount to convert.
  name: from_amount
  type: number
- description: Target amount after conversion.
  name: to_amount
  type: number
- description: Timestamp when the quote expires.
  name: expires_at
  type: string
- description: Quote creation timestamp.
  name: created_at
  type: string
provider_name: Airwallex
provider_slug: airwallex
schema_file: json-schema/airwallex-fx-quote-schema.json
slug: airwallex-fx-quote
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-fx-quote-schema.json\",\n  \"title\": \"FxQuote\",\n  \"description\": \"An Airwallex foreign exchange rate quote for currency conversion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quote_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique quote identifier.\",\n      \"example\": \"qte_abc123\"\n    },\n    \"from_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Source currency ISO 4217 code.\",\n      \"example\": \"USD\"\n    },\n    \"to_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Target currency ISO 4217 code.\",\n      \"example\": \"GBP\"\n    },\n    \"rate\": {\n      \"type\": \"number\",\n      \"description\": \"Quoted exchange rate (from_currency to to_currency).\",\n      \"example\": 0.7825\n    },\n    \"from_amount\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Source amount to convert.\",\n      \"example\": 1000.00\n    },\n    \"to_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Target amount after conversion.\",\n      \"example\": 782.50\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the quote expires.\",\n      \"example\": \"2026-04-19T10:32:00Z\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Quote creation timestamp.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  },\n  \"required\": [\"quote_id\", \"from_currency\", \"to_currency\", \"rate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-fx-quote-schema.json
tags:
- Cross-Border Payments
- FinTech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
title: FxQuote
---
