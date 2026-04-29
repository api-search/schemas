---
description: SplitAmount schema from Adyen API
layout: schema
name: SplitAmount
properties_list:
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). By default, this is the original payment currency.
  name: currency
  type: string
- description: The value of the split amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-split-amount-schema.json
slug: checkout-split-amount
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-split-amount-schema.json\",\n  \"title\": \"SplitAmount\",\n  \"description\": \"SplitAmount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). By default, this is the original payment currency.\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The value of the split amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-split-amount-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SplitAmount
---
