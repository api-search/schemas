---
description: BRLocalAccountIdentification schema from Adyen API
layout: schema
name: BRLocalAccountIdentification
properties_list:
- description: The bank account number (without separators or whitespace).
  name: accountNumber
  type: string
- description: The 3-digit Brazilian bank code (with leading zeros).
  name: bankCode
  type: string
- description: The bank account branch number (without separators or whitespace).
  name: branchNumber
  type: string
- description: '**brLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-br-local-account-identification-schema.json
slug: accounting-notifications-br-local-account-identification
source_filename: accounting-notifications-br-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-br-local-account-identification-schema.json\",\n  \"title\": \"BRLocalAccountIdentification\",\n  \"description\": \"BRLocalAccountIdentification schema from Adyen API\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The bank account number (without separators or whitespace).\",\n      \"maxLength\": 10,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"bankCode\": {\n      \"description\": \"The 3-digit Brazilian bank code (with leading zeros).\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"branchNumber\": {\n      \"description\": \"The bank account branch number (without separators or whitespace).\",\n      \"maxLength\": 4,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"\
  type\": {\n      \"default\": \"brLocal\",\n      \"description\": \"**brLocal**\",\n      \"enum\": [\n        \"brLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"branchNumber\",\n    \"accountNumber\",\n    \"bankCode\"\n  ],\n  \"additionalProperties\": false,\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-br-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BRLocalAccountIdentification
---
