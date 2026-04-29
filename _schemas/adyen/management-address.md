---
description: Address schema from Adyen API
layout: schema
name: Address
properties_list:
- description: The name of the city.
  name: city
  type: string
- description: The name of the company.
  name: companyName
  type: string
- description: The two-letter country code, in [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format.
  name: country
  type: string
- description: The postal code.
  name: postalCode
  type: string
- description: 'The state or province as defined in [ISO 3166-2](https://www.iso.org/standard/72483.html). For example, **ON** for Ontario, Canada. Applicable for the following countries: - Australia - Brazil - Canad'
  name: stateOrProvince
  type: string
- description: The name of the street, and the house or building number.
  name: streetAddress
  type: string
- description: Additional address details, if any.
  name: streetAddress2
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-address-schema.json
slug: management-address
source_filename: management-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city.\",\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"description\": \"The name of the company.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-letter country code, in [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The postal code.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The state or province as defined in [ISO 3166-2](https://www.iso.org/standard/72483.html).\
  \ For example, **ON** for Ontario, Canada. \\n\\nApplicable for the following countries:\\n- Australia\\n- Brazil\\n- Canada\\n- India\\n- Mexico\\n- New Zealand\\n- United States\",\n      \"type\": \"string\"\n    },\n    \"streetAddress\": {\n      \"description\": \"The name of the street, and the house or building number.\",\n      \"type\": \"string\"\n    },\n    \"streetAddress2\": {\n      \"description\": \"Additional address details, if any.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Address
---
