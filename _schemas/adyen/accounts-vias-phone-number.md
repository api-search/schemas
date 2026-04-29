---
description: ViasPhoneNumber schema from Adyen API
layout: schema
name: ViasPhoneNumber
properties_list:
- description: The two-character country code of the phone number. >The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').
  name: phoneCountryCode
  type: string
- description: The phone number. >The inclusion of the phone number country code is not necessary.
  name: phoneNumber
  type: string
- description: 'The type of the phone number. >The following values are permitted: `Landline`, `Mobile`, `SIP`, `Fax`.'
  name: phoneType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-vias-phone-number-schema.json
slug: accounts-vias-phone-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-phone-number-schema.json\",\n  \"title\": \"ViasPhoneNumber\",\n  \"description\": \"ViasPhoneNumber schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneCountryCode\": {\n      \"description\": \"The two-character country code of the phone number.\\n>The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number.\\n>The inclusion of the phone number country code is not necessary.\",\n      \"type\": \"string\"\n    },\n    \"phoneType\": {\n      \"description\": \"The type of the phone number.\\n>The following values are permitted: `Landline`, `Mobile`, `SIP`, `Fax`.\",\n      \"enum\": [\n        \"Fax\",\n        \"Landline\",\n        \"Mobile\",\n\
  \        \"SIP\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-phone-number-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ViasPhoneNumber
---
