---
description: StoredValueVoidRequest schema from Adyen API
layout: schema
name: StoredValueVoidRequest
properties_list:
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The original pspReference of the payment to modify.
  name: originalReference
  type: string
- description: 'Your reference for the payment modification. This reference is visible in Customer Area and in reports. Maximum length: 80 characters.'
  name: reference
  type: string
- description: The physical store, for which this payment is processed.
  name: store
  type: string
- description: The reference of the tender.
  name: tenderReference
  type: string
- description: The unique ID of a POS terminal.
  name: uniqueTerminalId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/stored-value-stored-value-void-request-schema.json
slug: stored-value-stored-value-void-request
source_filename: stored-value-stored-value-void-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-void-request-schema.json\",\n  \"title\": \"StoredValueVoidRequest\",\n  \"description\": \"StoredValueVoidRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"The original pspReference of the payment to modify.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment modification. This reference is visible in Customer Area and in reports.\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"The physical store, for\
  \ which this payment is processed.\",\n      \"maxLength\": 16,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"tenderReference\": {\n      \"description\": \"The reference of the tender.\",\n      \"type\": \"string\"\n    },\n    \"uniqueTerminalId\": {\n      \"description\": \"The unique ID of a POS terminal.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"originalReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-void-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueVoidRequest
---
