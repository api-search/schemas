---
description: BankAccountInfo schema from Adyen API
layout: schema
name: BankAccountInfo
properties_list:
- description: The address of the bank account owner.
  name: address
  type: object
- description: The international bank account number as defined in the [ISO-13616](https://www.iso.org/standard/81090.html) standard.
  name: iban
  type: string
- description: The name of the bank account owner.
  name: ownerName
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-bank-account-info-schema.json
slug: notification-webhooks-bank-account-info
source_filename: notification-webhooks-bank-account-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bank-account-info-schema.json\",\n  \"title\": \"BankAccountInfo\",\n  \"description\": \"BankAccountInfo schema from Adyen API\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the bank account owner.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"iban\": {\n      \"description\": \"The international bank account number as defined in the [ISO-13616](https://www.iso.org/standard/81090.html) standard.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"The name of the bank account owner.\",\n      \"$ref\": \"#/components/schemas/Name-2\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bank-account-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountInfo
---
