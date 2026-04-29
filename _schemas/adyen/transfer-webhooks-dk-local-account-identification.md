---
description: DKLocalAccountIdentification schema from Adyen API
layout: schema
name: DKLocalAccountIdentification
properties_list:
- description: The 4-10 digits bank account number (Kontonummer) (without separators or whitespace).
  name: accountNumber
  type: string
- description: The 4-digit bank code (Registreringsnummer) (without separators or whitespace).
  name: bankCode
  type: string
- description: '**dkLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-dk-local-account-identification-schema.json
slug: transfer-webhooks-dk-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-dk-local-account-identification-schema.json\",\n  \"title\": \"DKLocalAccountIdentification\",\n  \"description\": \"DKLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 4-10 digits bank account number (Kontonummer) (without separators or whitespace).\",\n      \"maxLength\": 10,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"bankCode\": {\n      \"description\": \"The 4-digit bank code (Registreringsnummer) (without separators or whitespace).\",\n      \"maxLength\": 4,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"dkLocal\",\n      \"description\": \"**dkLocal**\",\n      \"enum\": [\n        \"dkLocal\"\n      ],\n \
  \     \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"bankCode\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-dk-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DKLocalAccountIdentification
---
