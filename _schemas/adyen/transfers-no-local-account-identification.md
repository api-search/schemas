---
description: NOLocalAccountIdentification schema from Adyen API
layout: schema
name: NOLocalAccountIdentification
properties_list:
- description: The 11-digit bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: '**noLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-no-local-account-identification-schema.json
slug: transfers-no-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-no-local-account-identification-schema.json\",\n  \"title\": \"NOLocalAccountIdentification\",\n  \"description\": \"NOLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 11-digit bank account number, without separators or whitespace.\",\n      \"maxLength\": 11,\n      \"minLength\": 11,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"noLocal\",\n      \"description\": \"**noLocal**\",\n      \"enum\": [\n        \"noLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-no-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NOLocalAccountIdentification
---
