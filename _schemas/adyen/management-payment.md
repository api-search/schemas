---
description: Payment schema from Adyen API
layout: schema
name: Payment
properties_list:
- description: The default currency for contactless payments on the payment terminal, as the three-letter [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code.
  name: contactlessCurrency
  type: string
- description: Hides the minor units for the listed [ISO currency codes](https://en.wikipedia.org/wiki/ISO_4217).
  name: hideMinorUnitsInCurrencies
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payment-schema.json
slug: management-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-schema.json\",\n  \"title\": \"Payment\",\n  \"description\": \"Payment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactlessCurrency\": {\n      \"description\": \"The default currency for contactless payments on the payment terminal, as the three-letter [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code.\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"hideMinorUnitsInCurrencies\": {\n      \"description\": \"Hides the minor units for the listed [ISO currency codes](https://en.wikipedia.org/wiki/ISO_4217).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Payment
---
