---
description: Address schema from Adyen API
layout: schema
name: Address
properties_list:
- description: 'The name of the city. Maximum length: 3000 characters.'
  name: city
  type: string
- description: The two-character ISO-3166-1 alpha-2 country code. For example, **US**. > If you don't know the country or are not collecting the country from the shopper, provide `country` as `ZZ`.
  name: country
  type: string
- description: 'The number or name of the house. Maximum length: 3000 characters.'
  name: houseNumberOrName
  type: string
- description: A maximum of five digits for an address in the US, or a maximum of ten characters for an address in all other countries.
  name: postalCode
  type: string
- description: The two-character ISO 3166-2 state or province code. For example, **CA** in the US or **ON** in Canada. > Required for the US and Canada.
  name: stateOrProvince
  type: string
- description: 'The name of the street. Maximum length: 3000 characters. > The house number should not be included in this field; it should be separately provided via `houseNumberOrName`.'
  name: street
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-address-schema.json
slug: recurring-address
source_filename: recurring-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city. Maximum length: 3000 characters.\",\n      \"maxLength\": 3000,\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code. For example, **US**.\\n> If you don't know the country or are not collecting the country from the shopper, provide `country` as `ZZ`.\",\n      \"type\": \"string\"\n    },\n    \"houseNumberOrName\": {\n      \"description\": \"The number or name of the house. Maximum length: 3000 characters.\",\n      \"maxLength\": 3000,\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\"\
  : \"A maximum of five digits for an address in the US, or a maximum of ten characters for an address in all other countries.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The two-character ISO 3166-2 state or province code. For example, **CA** in the US or **ON** in Canada.\\n> Required for the US and Canada.\",\n      \"type\": \"string\"\n    },\n    \"street\": {\n      \"description\": \"The name of the street. Maximum length: 3000 characters.\\n> The house number should not be included in this field; it should be separately provided via `houseNumberOrName`.\",\n      \"maxLength\": 3000,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"street\",\n    \"houseNumberOrName\",\n    \"city\",\n    \"postalCode\",\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Address
---
