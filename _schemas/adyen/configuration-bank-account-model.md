---
description: BankAccountModel schema from Adyen API
layout: schema
name: BankAccountModel
properties_list:
- description: Form factor of the bank account - **virtual** or **physical** (default)
  name: formFactor
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-bank-account-model-schema.json
slug: configuration-bank-account-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-model-schema.json\",\n  \"title\": \"BankAccountModel\",\n  \"description\": \"BankAccountModel schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formFactor\": {\n      \"description\": \"Form factor of the bank account - **virtual** or **physical** (default)\",\n      \"enum\": [\n        \"physical\",\n        \"unknown\",\n        \"virtual\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-model-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountModel
---
