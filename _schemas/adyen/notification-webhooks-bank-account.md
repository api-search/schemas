---
description: BankAccount schema from Adyen API
layout: schema
name: BankAccount
properties_list:
- description: The [International Bank Account Number](https://en.wikipedia.org/wiki/International_Bank_Account_Number) (IBAN).
  name: iban
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-bank-account-schema.json
slug: notification-webhooks-bank-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bank-account-schema.json\",\n  \"title\": \"BankAccount\",\n  \"description\": \"BankAccount schema from Adyen API\",\n  \"properties\": {\n    \"iban\": {\n      \"description\": \"The [International Bank Account Number](https://en.wikipedia.org/wiki/International_Bank_Account_Number) (IBAN).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"iban\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bank-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccount
---
