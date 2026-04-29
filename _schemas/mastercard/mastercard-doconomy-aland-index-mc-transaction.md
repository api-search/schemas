---
description: This object holds data corresponding to a single payment transaction.
layout: schema
name: MCTransaction
properties_list:
- description: Merchant category code of a payment transaction that uniquely defines a merchant business.
  name: mcc
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-transaction-schema.json
slug: mastercard-doconomy-aland-index-mc-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCTransaction\",\n  \"type\": \"object\",\n  \"description\": \"This object holds data corresponding to a single payment transaction.\",\n  \"properties\": {\n    \"mcc\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant category code of a payment transaction that uniquely defines a merchant business.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-transaction-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCTransaction
---
