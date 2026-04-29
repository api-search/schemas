---
description: Currency definition with exchange rate information
layout: schema
name: Currency
properties_list:
- description: ISO 4217 currency code
  name: currencyCode
  type: string
- description: Full currency name
  name: currencyName
  type: string
- description: ISO 4217 numeric code
  name: numericCode
  type: string
- description: Number of decimal places
  name: decimalPlaces
  type: integer
- description: Current buy exchange rate
  name: buyRate
  type: number
- description: Current sell exchange rate
  name: sellRate
  type: number
- description: Mid-market exchange rate
  name: midRate
  type: number
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-currency-schema.json
slug: temenos-transact-core-banking-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Currency\",\n  \"type\": \"object\",\n  \"description\": \"Currency definition with exchange rate information\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"currencyName\": {\n      \"type\": \"string\",\n      \"description\": \"Full currency name\"\n    },\n    \"numericCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 numeric code\"\n    },\n    \"decimalPlaces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of decimal places\"\n    },\n    \"buyRate\": {\n      \"type\": \"number\",\n      \"description\": \"Current buy exchange rate\"\n    },\n    \"sellRate\": {\n      \"type\": \"number\",\n      \"description\": \"Current sell exchange rate\"\n    },\n    \"midRate\": {\n      \"type\": \"number\",\n      \"description\": \"Mid-market exchange rate\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-currency-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Currency
---
