---
description: Phone schema from Adyen API
layout: schema
name: Phone
properties_list:
- description: 'Country code. Length: 1–3 characters.'
  name: cc
  type: string
- description: 'Subscriber number. Maximum length: 15 characters.'
  name: subscriber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-phone-schema.json
slug: checkout-phone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-phone-schema.json\",\n  \"title\": \"Phone\",\n  \"description\": \"Phone schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cc\": {\n      \"description\": \"Country code. Length: 1\\u20133 characters.\",\n      \"maxLength\": 3,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"subscriber\": {\n      \"description\": \"Subscriber number. Maximum length: 15 characters.\",\n      \"maxLength\": 15,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-phone-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Phone
---
