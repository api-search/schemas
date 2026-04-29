---
description: HKLocalAccountIdentification schema from Adyen API
layout: schema
name: HKLocalAccountIdentification
properties_list:
- description: The 9- to 15-character bank account number (alphanumeric), without separators or whitespace. Starts with the 3-digit branch code.
  name: accountNumber
  type: string
- description: The 3-digit clearing code, without separators or whitespace.
  name: clearingCode
  type: string
- description: '**hkLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-hk-local-account-identification-schema.json
slug: transfer-webhooks-hk-local-account-identification
source_filename: transfer-webhooks-hk-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-hk-local-account-identification-schema.json\",\n  \"title\": \"HKLocalAccountIdentification\",\n  \"description\": \"HKLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 9- to 15-character bank account number (alphanumeric), without separators or whitespace. Starts with the 3-digit branch code.\",\n      \"maxLength\": 15,\n      \"minLength\": 9,\n      \"type\": \"string\"\n    },\n    \"clearingCode\": {\n      \"description\": \"The 3-digit clearing code, without separators or whitespace.\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"hkLocal\",\n      \"description\": \"**hkLocal**\",\n      \"enum\": [\n   \
  \     \"hkLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"clearingCode\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-hk-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: HKLocalAccountIdentification
---
