---
description: AdditionalInfo Response
layout: schema
name: AdditionalInfo
properties_list:
- description: Balance of requested account
  name: balance
  type: string
- description: Currency
  name: currency
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-community-pass-payments-additional-info-schema.json
slug: mastercard-community-pass-payments-additional-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AdditionalInfo\",\n  \"type\": \"object\",\n  \"description\": \"AdditionalInfo Response\",\n  \"properties\": {\n    \"balance\": {\n      \"type\": \"string\",\n      \"description\": \"Balance of requested account\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-community-pass-payments-additional-info-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AdditionalInfo
---
