---
description: SGLocalAccountIdentification schema from Adyen API
layout: schema
name: SGLocalAccountIdentification
properties_list:
- description: The 4- to 19-digit bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: The bank's 8- or 11-character BIC or SWIFT code.
  name: bic
  type: string
- description: '**sgLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-sg-local-account-identification-schema.json
slug: configuration-sg-local-account-identification
source_filename: configuration-sg-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sg-local-account-identification-schema.json\",\n  \"title\": \"SGLocalAccountIdentification\",\n  \"description\": \"SGLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 4- to 19-digit bank account number, without separators or whitespace.\",\n      \"maxLength\": 19,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"bic\": {\n      \"description\": \"The bank's 8- or 11-character BIC or SWIFT code.\",\n      \"maxLength\": 11,\n      \"minLength\": 8,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"sgLocal\",\n      \"description\": \"**sgLocal**\",\n      \"enum\": [\n        \"sgLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\"\
  : [\n    \"accountNumber\",\n    \"bic\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sg-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SGLocalAccountIdentification
---
