---
description: ''
layout: schema
name: Address
properties_list:
- description: The first line of the street part in the structured address.
  name: addressLine1
  type: string
- description: The second line of the street part in the structured address.
  name: addressLine2
  type: string
- description: The name of the city in the structured address.
  name: addressCity
  type: string
- description: The state/province/parent subdivision code of the structured address.
  name: addressState
  type: string
- description: The postal code of the structured address.
  name: addressPostCode
  type: string
- description: 'The ISO-3166-1 numeric country code of the billing or shipping address requested by the cardholder. See: [ISO-3166](https://www.nationsonline.org/oneworld/country_code_list.htm).'
  name: addressCountry
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-address-schema.json
slug: mastercard-identity-insights-for-transactions-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the street part in the structured address.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"The second line of the street part in the structured address.\"\n    },\n    \"addressCity\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the city in the structured address.\"\n    },\n    \"addressState\": {\n      \"type\": \"string\",\n      \"description\": \"The state/province/parent subdivision code of the structured address.\"\n    },\n    \"addressPostCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the structured address.\"\n    },\n    \"addressCountry\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO-3166-1 numeric country\
  \ code of the billing or shipping address requested by the cardholder. See: [ISO-3166](https://www.nationsonline.org/oneworld/country_code_list.htm).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Address
---
