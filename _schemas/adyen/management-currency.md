---
description: Currency schema from Adyen API
layout: schema
name: Currency
properties_list:
- description: Surcharge amount per transaction, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: amount
  type: integer
- description: Three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). For example, **AUD**.
  name: currencyCode
  type: string
- description: Surcharge percentage per transaction. The maximum number of decimal places is two. For example, **1%** or **2.27%**.
  name: percentage
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-currency-schema.json
slug: management-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-currency-schema.json\",\n  \"title\": \"Currency\",\n  \"description\": \"Currency schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"Surcharge amount per transaction, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"currencyCode\": {\n      \"description\": \"Three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). For example, **AUD**.\",\n      \"type\": \"string\"\n    },\n    \"percentage\": {\n      \"description\": \"Surcharge percentage per transaction. The maximum number of decimal places is two. For example, **1%** or **2.27%**.\",\n      \"format\": \"double\",\n      \"type\": \"\
  number\"\n    }\n  },\n  \"required\": [\n    \"currencyCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-currency-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Currency
---
