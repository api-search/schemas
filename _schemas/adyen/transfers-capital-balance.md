---
description: CapitalBalance schema from Adyen API
layout: schema
name: CapitalBalance
properties_list:
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).
  name: currency
  type: string
- description: Fee amount.
  name: fee
  type: integer
- description: Principal amount.
  name: principal
  type: integer
- description: Total amount. A sum of principal amount and fee amount.
  name: total
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-capital-balance-schema.json
slug: transfers-capital-balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-balance-schema.json\",\n  \"title\": \"CapitalBalance\",\n  \"description\": \"CapitalBalance schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"type\": \"string\"\n    },\n    \"fee\": {\n      \"description\": \"Fee amount.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"principal\": {\n      \"description\": \"Principal amount.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"description\": \"Total amount. A sum of principal amount and fee amount.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\":\
  \ [\n    \"principal\",\n    \"fee\",\n    \"total\",\n    \"currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-balance-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapitalBalance
---
