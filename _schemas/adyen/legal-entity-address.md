---
description: Address schema from Adyen API
layout: schema
name: Address
properties_list:
- description: The name of the city. Required if `stateOrProvince` is provided. If you specify the city, you must also send `postalCode` and `street`.
  name: city
  type: string
- description: The two-letter [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code.
  name: country
  type: string
- description: Postal code. Required if `stateOrProvince` and/or `city` is provided.
  name: postalCode
  type: string
- description: The two-letter ISO 3166-2 state or province code. For example, **CA** in the US. If you specify the state or province, you must also send `city`, `postalCode`, and `street`.
  name: stateOrProvince
  type: string
- description: The name of the street, and the house or building number. Required if `stateOrProvince` and/or `city` is provided.
  name: street
  type: string
- description: The apartment, unit, or suite number.
  name: street2
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-address-schema.json
slug: legal-entity-address
source_filename: legal-entity-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city. Required if `stateOrProvince` is provided.\\n\\nIf you specify the city, you must also send `postalCode` and `street`.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-letter [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"Postal code. Required if `stateOrProvince` and/or `city` is provided.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The two-letter ISO 3166-2 state or province\
  \ code. For example, **CA** in the US.\\n\\nIf you specify the state or province, you must also send `city`, `postalCode`, and `street`.\",\n      \"type\": \"string\"\n    },\n    \"street\": {\n      \"description\": \"The name of the street, and the house or building number. Required if `stateOrProvince` and/or `city` is provided.\",\n      \"type\": \"string\"\n    },\n    \"street2\": {\n      \"description\": \"The apartment, unit, or suite number.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Address
---
