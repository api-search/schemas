---
description: DeliveryAddress schema from Adyen API
layout: schema
name: DeliveryAddress
properties_list:
- description: The name of the city.
  name: city
  type: string
- description: The two-character ISO-3166-1 alpha-2 country code. For example, **US**. >If you don't know the country or are not collecting the country from the shopper, provide `country` as `ZZ`.
  name: country
  type: string
- description: The street name. For example, if the address is "Rokin 49", provide "Rokin".
  name: line1
  type: string
- description: The house number or name. For example, if the address is "Rokin 49", provide "49".
  name: line2
  type: string
- description: Optional information about the address.
  name: line3
  type: string
- description: 'The postal code. Maximum length: * 5 digits for an address in the US. * 10 characters for an address in all other countries.'
  name: postalCode
  type: string
- description: The two-letterISO 3166-2 state or province code. For example, **CA** in the US or **ON** in Canada. > Required for the US and Canada.
  name: stateOrProvince
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-delivery-address-schema.json
slug: configuration-delivery-address
source_filename: configuration-delivery-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-delivery-address-schema.json\",\n  \"title\": \"DeliveryAddress\",\n  \"description\": \"DeliveryAddress schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code. For example, **US**.\\n>If you don't know the country or are not collecting the country from the shopper, provide `country` as `ZZ`.\",\n      \"type\": \"string\"\n    },\n    \"line1\": {\n      \"description\": \"The street name. For example, if the address is \\\"Rokin 49\\\", provide \\\"Rokin\\\".\",\n      \"type\": \"string\"\n    },\n    \"line2\": {\n      \"description\": \"The house number or name. For example, if the\
  \ address is \\\"Rokin 49\\\", provide \\\"49\\\".\",\n      \"type\": \"string\"\n    },\n    \"line3\": {\n      \"description\": \"Optional information about the address.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The postal code.\\nMaximum length:\\n* 5 digits for an address in the US.\\n* 10 characters for an address in all other countries.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The two-letterISO 3166-2 state or province code. For example, **CA** in the US or **ON** in Canada.\\n> Required for the US and Canada.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-delivery-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeliveryAddress
---
