---
description: PLLocalAccountIdentification schema from Adyen API
layout: schema
name: PLLocalAccountIdentification
properties_list:
- description: The 26-digit bank account number ([Numer rachunku](https://pl.wikipedia.org/wiki/Numer_Rachunku_Bankowego)), without separators or whitespace.
  name: accountNumber
  type: string
- description: '**plLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-pl-local-account-identification-schema.json
slug: configuration-pl-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pl-local-account-identification-schema.json\",\n  \"title\": \"PLLocalAccountIdentification\",\n  \"description\": \"PLLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 26-digit bank account number ([Numer rachunku](https://pl.wikipedia.org/wiki/Numer_Rachunku_Bankowego)), without separators or whitespace.\",\n      \"maxLength\": 26,\n      \"minLength\": 26,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"plLocal\",\n      \"description\": \"**plLocal**\",\n      \"enum\": [\n        \"plLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pl-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PLLocalAccountIdentification
---
