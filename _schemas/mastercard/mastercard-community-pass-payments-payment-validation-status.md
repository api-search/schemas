---
description: Validation Response
layout: schema
name: PaymentValidationStatus
properties_list:
- description: Account Id
  name: accountId
  type: string
- description: Account Name
  name: accountName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-community-pass-payments-payment-validation-status-schema.json
slug: mastercard-community-pass-payments-payment-validation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentValidationStatus\",\n  \"type\": \"object\",\n  \"description\": \"Validation Response\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account Id\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account Name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-community-pass-payments-payment-validation-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PaymentValidationStatus
---
