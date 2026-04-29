---
description: PhoneNumber schema from Adyen API
layout: schema
name: PhoneNumber
properties_list:
- description: The two-character ISO-3166-1 alpha-2 country code of the phone number. For example, **US** or **NL**.
  name: phoneCountryCode
  type: string
- description: The phone number. The inclusion of the phone number country code is not necessary.
  name: phoneNumber
  type: string
- description: 'The type of the phone number. Possible values: **Landline**, **Mobile**, **SIP**, **Fax**.'
  name: phoneType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-phone-number-schema.json
slug: configuration-phone-number
source_filename: configuration-phone-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-phone-number-schema.json\",\n  \"title\": \"PhoneNumber\",\n  \"description\": \"PhoneNumber schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneCountryCode\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code of the phone number.\\nFor example, **US** or **NL**.\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number.\\nThe inclusion of the phone number country code is not necessary.\",\n      \"type\": \"string\"\n    },\n    \"phoneType\": {\n      \"description\": \"The type of the phone number.\\nPossible values: **Landline**, **Mobile**, **SIP**, **Fax**.\",\n      \"enum\": [\n        \"Fax\",\n        \"Landline\",\n        \"Mobile\",\n        \"SIP\"\n      ],\n      \"type\": \"string\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-phone-number-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PhoneNumber
---
