---
description: ViasAddress schema from Adyen API
layout: schema
name: ViasAddress
properties_list:
- description: The name of the city. Required if the `houseNumberOrName`, `street`, `postalCode`, or `stateOrProvince` are provided.
  name: city
  type: string
- description: The two-character country code of the address in ISO-3166-1 alpha-2 format. For example, **NL**.
  name: country
  type: string
- description: The number or name of the house.
  name: houseNumberOrName
  type: string
- description: 'The postal code. Required if the `houseNumberOrName`, `street`, `city`, or `stateOrProvince` are provided. Maximum length: * 5 digits for addresses in the US. * 10 characters for all other countries.'
  name: postalCode
  type: string
- description: 'The abbreviation of the state or province. Required if the `houseNumberOrName`, `street`, `city`, or `postalCode` are provided. Maximum length: * 2 characters for addresses in the US or Canada. * 3 ch'
  name: stateOrProvince
  type: string
- description: The name of the street. Required if the `houseNumberOrName`, `city`, `postalCode`, or `stateOrProvince` are provided.
  name: street
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-vias-address-schema.json
slug: accounts-vias-address
source_filename: accounts-vias-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-address-schema.json\",\n  \"title\": \"ViasAddress\",\n  \"description\": \"ViasAddress schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city. Required if the `houseNumberOrName`, `street`, `postalCode`, or `stateOrProvince` are provided.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-character country code of the address in ISO-3166-1 alpha-2 format. For example, **NL**.\",\n      \"type\": \"string\"\n    },\n    \"houseNumberOrName\": {\n      \"description\": \"The number or name of the house.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The postal code. Required if the `houseNumberOrName`, `street`, `city`, or `stateOrProvince`\
  \ are provided.\\n\\nMaximum length:\\n\\n* 5 digits for addresses in the US.\\n\\n* 10 characters for all other countries.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The abbreviation of the state or province. Required if the `houseNumberOrName`, `street`, `city`, or `postalCode` are provided. \\n\\nMaximum length:\\n\\n* 2 characters for addresses in the US or Canada.\\n\\n* 3 characters for all other countries.\\n\",\n      \"type\": \"string\"\n    },\n    \"street\": {\n      \"description\": \"The name of the street. Required if the `houseNumberOrName`, `city`, `postalCode`, or `stateOrProvince` are provided.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ViasAddress
---
