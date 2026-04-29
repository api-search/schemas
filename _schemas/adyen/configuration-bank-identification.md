---
description: BankIdentification schema from Adyen API
layout: schema
name: BankIdentification
properties_list:
- description: ''
  name: country
  type: string
- description: ''
  name: identification
  type: string
- description: ''
  name: identificationType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-bank-identification-schema.json
slug: configuration-bank-identification
source_filename: configuration-bank-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-identification-schema.json\",\n  \"title\": \"BankIdentification\",\n  \"description\": \"BankIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"identification\": {\n      \"type\": \"string\"\n    },\n    \"identificationType\": {\n      \"enum\": [\n        \"iban\",\n        \"routingNumber\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankIdentification
---
