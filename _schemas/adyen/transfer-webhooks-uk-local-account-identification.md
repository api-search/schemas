---
description: UKLocalAccountIdentification schema from Adyen API
layout: schema
name: UKLocalAccountIdentification
properties_list:
- description: The 8-digit bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: The 6-digit [sort code](https://en.wikipedia.org/wiki/Sort_code), without separators or whitespace.
  name: sortCode
  type: string
- description: '**ukLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-uk-local-account-identification-schema.json
slug: transfer-webhooks-uk-local-account-identification
source_filename: transfer-webhooks-uk-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-uk-local-account-identification-schema.json\",\n  \"title\": \"UKLocalAccountIdentification\",\n  \"description\": \"UKLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 8-digit bank account number, without separators or whitespace.\",\n      \"maxLength\": 8,\n      \"minLength\": 8,\n      \"type\": \"string\"\n    },\n    \"sortCode\": {\n      \"description\": \"The 6-digit [sort code](https://en.wikipedia.org/wiki/Sort_code), without separators or whitespace.\",\n      \"maxLength\": 6,\n      \"minLength\": 6,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"ukLocal\",\n      \"description\": \"**ukLocal**\",\n      \"enum\": [\n        \"ukLocal\"\n      ],\n \
  \     \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"sortCode\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-uk-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UKLocalAccountIdentification
---
