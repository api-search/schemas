---
description: Address schema from Adyen API
layout: schema
name: Address
properties_list:
- description: ''
  name: city
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: stateOrProvince
  type: string
- description: ''
  name: streetAddress
  type: string
- description: ''
  name: streetAddress2
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-address-schema.json
slug: pos-terminal-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"type\": \"string\"\n    },\n    \"streetAddress\": {\n      \"type\": \"string\"\n    },\n    \"streetAddress2\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Address
---
