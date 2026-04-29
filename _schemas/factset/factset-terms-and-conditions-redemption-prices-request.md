---
description: ''
layout: schema
name: redemptionPricesRequest
properties_list:
- description: List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S). **ID LIMIT = 250** *per request*.
  name: ids
  type: array
- description: Filters the list of Redemption Prices Categories - * **CALL** = Call prices. * **PUT** = Put prices. * **SF** = Sinking Fund prices.
  name: categories
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-redemption-prices-request-schema.json
slug: factset-terms-and-conditions-redemption-prices-request
source_filename: factset-terms-and-conditions-redemption-prices-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"redemptionPricesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S).\\n\\n**ID LIMIT = 250** *per request*.\\n\"\n    },\n    \"categories\": {\n      \"type\": \"string\",\n      \"description\": \"Filters the list of Redemption Prices Categories -\\n  * **CALL** = Call prices.\\n  * **PUT** = Put prices.\\n  * **SF** = Sinking Fund prices.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-redemption-prices-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: redemptionPricesRequest
---
