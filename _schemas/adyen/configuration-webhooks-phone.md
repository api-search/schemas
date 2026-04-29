---
description: Phone schema from Adyen API
layout: schema
name: Phone
properties_list:
- description: The full phone number provided as a single string. For example, **"0031 6 11 22 33 44"**, **"+316/1122-3344"**, or **"(0031) 611223344"**.
  name: number
  type: string
- description: 'Type of phone number. Possible values: **Landline**, **Mobile**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-phone-schema.json
slug: configuration-webhooks-phone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-phone-schema.json\",\n  \"title\": \"Phone\",\n  \"description\": \"Phone schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"description\": \"The full phone number provided as a single string. \\nFor example, **\\\"0031 6 11 22 33 44\\\"**, **\\\"+316/1122-3344\\\"**, \\n\\n or **\\\"(0031) 611223344\\\"**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of phone number.\\nPossible values: \\n**Landline**, **Mobile**.\\n\",\n      \"enum\": [\n        \"Landline\",\n        \"Mobile\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"number\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-phone-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Phone
---
