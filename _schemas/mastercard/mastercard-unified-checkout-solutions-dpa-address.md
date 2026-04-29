---
description: The Digital Payment Application (DPA) business address.
layout: schema
name: DpaAddress
properties_list:
- description: Name of the address
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
- description: The city/town of the address.
  name: city
  type: string
- description: The state of the address. Use 2-character state designation for USA and Canada addresses.
  name: state
  type: string
- description: ISO 3166 alpha 2 country code. Note that for the UK the correct ISO code is "GB".
  name: countryCode
  type: string
- description: Zipcode for the region.
  name: zip
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-dpa-address-schema.json
slug: mastercard-unified-checkout-solutions-dpa-address
source_filename: mastercard-unified-checkout-solutions-dpa-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaAddress\",\n  \"type\": \"object\",\n  \"description\": \"The Digital Payment Application (DPA) business address.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the address\"\n    },\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the address.\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the address.\"\n    },\n    \"line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city/town of the address.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the address. Use 2-character state designation for USA and Canada addresses.\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"ISO 3166 alpha 2 country code. Note that for the UK the correct ISO code is \\\"GB\\\".\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Zipcode for the region.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-dpa-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaAddress
---
