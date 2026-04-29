---
description: NumberAndBicAccountIdentification schema from Adyen API
layout: schema
name: NumberAndBicAccountIdentification
properties_list:
- description: The bank account number, without separators or whitespace. The length and format depends on the bank or country.
  name: accountNumber
  type: string
- description: Additional identification codes of the bank. Some banks may require these identifiers for cross-border transfers.
  name: additionalBankIdentification
  type: object
- description: The bank's 8- or 11-character BIC or SWIFT code.
  name: bic
  type: string
- description: '**numberAndBic**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-number-and-bic-account-identification-schema.json
slug: configuration-number-and-bic-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-number-and-bic-account-identification-schema.json\",\n  \"title\": \"NumberAndBicAccountIdentification\",\n  \"description\": \"NumberAndBicAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The bank account number, without separators or whitespace. The length and format depends on the bank or country.\",\n      \"maxLength\": 34,\n      \"type\": \"string\"\n    },\n    \"additionalBankIdentification\": {\n      \"description\": \"Additional identification codes of the bank. Some banks may require these identifiers for cross-border transfers.\",\n      \"$ref\": \"#/components/schemas/AdditionalBankIdentification\"\n    },\n    \"bic\": {\n      \"description\": \"The bank's 8- or 11-character BIC or SWIFT\
  \ code.\",\n      \"maxLength\": 11,\n      \"minLength\": 8,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"numberAndBic\",\n      \"description\": \"**numberAndBic**\",\n      \"enum\": [\n        \"numberAndBic\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"bic\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-number-and-bic-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NumberAndBicAccountIdentification
---
