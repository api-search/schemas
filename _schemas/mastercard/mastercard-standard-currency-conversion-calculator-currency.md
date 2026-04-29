---
description: ''
layout: schema
name: Currency
properties_list:
- description: The Alpha code for the currency.
  name: alphaCd
  type: string
- description: The full name of the currency.
  name: currNam
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-standard-currency-conversion-calculator-currency-schema.json
slug: mastercard-standard-currency-conversion-calculator-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Currency\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alphaCd\": {\n      \"type\": \"string\",\n      \"description\": \"The Alpha code for the currency.\"\n    },\n    \"currNam\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the currency.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-standard-currency-conversion-calculator-currency-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Currency
---
