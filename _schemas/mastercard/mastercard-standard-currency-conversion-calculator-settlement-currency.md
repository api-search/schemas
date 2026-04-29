---
description: ''
layout: schema
name: SettlementCurrency
properties_list:
- description: A list of settlement currencies
  name: currencies
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-standard-currency-conversion-calculator-settlement-currency-schema.json
slug: mastercard-standard-currency-conversion-calculator-settlement-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SettlementCurrency\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencies\": {\n      \"type\": \"array\",\n      \"description\": \"A list of settlement currencies\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-standard-currency-conversion-calculator-settlement-currency-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SettlementCurrency
---
