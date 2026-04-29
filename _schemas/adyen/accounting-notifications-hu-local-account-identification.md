---
description: HULocalAccountIdentification schema from Adyen API
layout: schema
name: HULocalAccountIdentification
properties_list:
- description: The 24-digit bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: '**huLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-hu-local-account-identification-schema.json
slug: accounting-notifications-hu-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-hu-local-account-identification-schema.json\",\n  \"title\": \"HULocalAccountIdentification\",\n  \"description\": \"HULocalAccountIdentification schema from Adyen API\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 24-digit bank account number, without separators or whitespace.\",\n      \"maxLength\": 24,\n      \"minLength\": 24,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"huLocal\",\n      \"description\": \"**huLocal**\",\n      \"enum\": [\n        \"huLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\"\n  ],\n  \"additionalProperties\": false,\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-hu-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: HULocalAccountIdentification
---
