---
description: The Digital Payment Application (DPA) business address.
layout: schema
name: Address
properties_list:
- description: Contact name for the address.
  name: name
  type: string
- description: First line of the address.
  name: line1
  type: string
- description: Second line of the address.
  name: line2
  type: string
- description: Third line of the address.
  name: line3
  type: string
- description: Address of city
  name: city
  type: string
- description: Address of state
  name: state
  type: string
- description: Address country code. ISO 3166 alpha 2 country code.
  name: countryCode
  type: string
- description: Address zip/postal code.
  name: zip
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-address-schema.json
slug: mastercard-checkout-solutions-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"description\": \"The Digital Payment Application (DPA) business address.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact name for the address.\"\n    },\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the address.\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the address.\"\n    },\n    \"line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"Address of city\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Address of state\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Address country code. ISO 3166 alpha 2 country\
  \ code.\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Address zip/postal code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Address
---
