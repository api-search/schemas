---
description: CALocalAccountIdentification schema from Adyen API
layout: schema
name: CALocalAccountIdentification
properties_list:
- description: The 5- to 12-digit bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: The 3-digit institution number, without separators or whitespace.
  name: institutionNumber
  type: string
- description: The 5-digit transit number, without separators or whitespace.
  name: transitNumber
  type: string
- description: '**caLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-ca-local-account-identification-schema.json
slug: accounting-notifications-ca-local-account-identification
source_filename: accounting-notifications-ca-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-ca-local-account-identification-schema.json\",\n  \"title\": \"CALocalAccountIdentification\",\n  \"description\": \"CALocalAccountIdentification schema from Adyen API\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 5- to 12-digit bank account number, without separators or whitespace.\",\n      \"maxLength\": 12,\n      \"minLength\": 5,\n      \"type\": \"string\"\n    },\n    \"institutionNumber\": {\n      \"description\": \"The 3-digit institution number, without separators or whitespace.\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"transitNumber\": {\n      \"description\": \"The 5-digit transit number, without separators or whitespace.\",\n      \"maxLength\": 5,\n      \"minLength\": 5,\n      \"type\"\
  : \"string\"\n    },\n    \"type\": {\n      \"default\": \"caLocal\",\n      \"description\": \"**caLocal**\",\n      \"enum\": [\n        \"caLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"institutionNumber\",\n    \"transitNumber\"\n  ],\n  \"additionalProperties\": false,\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-ca-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CALocalAccountIdentification
---
