---
description: SELocalAccountIdentification schema from Adyen API
layout: schema
name: SELocalAccountIdentification
properties_list:
- description: The 7- to 10-digit bank account number ([Bankkontonummer](https://sv.wikipedia.org/wiki/Bankkonto)), without the clearing number, separators, or whitespace.
  name: accountNumber
  type: string
- description: The 4- to 5-digit clearing number ([Clearingnummer](https://sv.wikipedia.org/wiki/Clearingnummer)), without separators or whitespace.
  name: clearingNumber
  type: string
- description: '**seLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-se-local-account-identification-schema.json
slug: transfer-webhooks-se-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-se-local-account-identification-schema.json\",\n  \"title\": \"SELocalAccountIdentification\",\n  \"description\": \"SELocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 7- to 10-digit bank account number ([Bankkontonummer](https://sv.wikipedia.org/wiki/Bankkonto)), without the clearing number, separators, or whitespace.\",\n      \"maxLength\": 10,\n      \"minLength\": 7,\n      \"type\": \"string\"\n    },\n    \"clearingNumber\": {\n      \"description\": \"The 4- to 5-digit clearing number ([Clearingnummer](https://sv.wikipedia.org/wiki/Clearingnummer)), without separators or whitespace.\",\n      \"maxLength\": 5,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"type\"\
  : {\n      \"default\": \"seLocal\",\n      \"description\": \"**seLocal**\",\n      \"enum\": [\n        \"seLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"clearingNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-se-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SELocalAccountIdentification
---
