---
description: AULocalAccountIdentification schema from Adyen API
layout: schema
name: AULocalAccountIdentification
properties_list:
- description: The bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: The 6-digit [Bank State Branch (BSB) code](https://en.wikipedia.org/wiki/Bank_state_branch), without separators or whitespace.
  name: bsbCode
  type: string
- description: '**auLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-au-local-account-identification-schema.json
slug: transfer-webhooks-au-local-account-identification
source_filename: transfer-webhooks-au-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-au-local-account-identification-schema.json\",\n  \"title\": \"AULocalAccountIdentification\",\n  \"description\": \"AULocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The bank account number, without separators or whitespace.\",\n      \"maxLength\": 9,\n      \"minLength\": 5,\n      \"type\": \"string\"\n    },\n    \"bsbCode\": {\n      \"description\": \"The 6-digit [Bank State Branch (BSB) code](https://en.wikipedia.org/wiki/Bank_state_branch), without separators or whitespace.\",\n      \"maxLength\": 6,\n      \"minLength\": 6,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"auLocal\",\n      \"description\": \"**auLocal**\",\n      \"enum\": [\n        \"auLocal\"\
  \n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"bsbCode\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-au-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AULocalAccountIdentification
---
