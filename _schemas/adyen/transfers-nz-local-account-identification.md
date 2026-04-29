---
description: NZLocalAccountIdentification schema from Adyen API
layout: schema
name: NZLocalAccountIdentification
properties_list:
- description: The 15-16 digit bank account number. The first 2 digits are the bank number, the next 4 digits are the branch number, the next 7 digits are the account number, and the final 2-3 digits are the suffix.
  name: accountNumber
  type: string
- description: '**nzLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-nz-local-account-identification-schema.json
slug: transfers-nz-local-account-identification
source_filename: transfers-nz-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-nz-local-account-identification-schema.json\",\n  \"title\": \"NZLocalAccountIdentification\",\n  \"description\": \"NZLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 15-16 digit bank account number. The first 2 digits are the bank number, the next 4 digits are the branch number, the next 7 digits are the account number, and the final 2-3 digits are the suffix.\",\n      \"maxLength\": 16,\n      \"minLength\": 15,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"nzLocal\",\n      \"description\": \"**nzLocal**\",\n      \"enum\": [\n        \"nzLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\"\n  ],\n  \"additionalProperties\"\
  : false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-nz-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NZLocalAccountIdentification
---
