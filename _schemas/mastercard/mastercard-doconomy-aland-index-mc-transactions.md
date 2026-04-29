---
description: Request object which holds all the payment transactions from API consumer for calculating transaction footprint.
layout: schema
name: MCTransactions
properties_list:
- description: ''
  name: transactions
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-transactions-schema.json
slug: mastercard-doconomy-aland-index-mc-transactions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCTransactions\",\n  \"type\": \"object\",\n  \"description\": \"Request object which holds all the payment transactions from API consumer for calculating transaction footprint.\",\n  \"properties\": {\n    \"transactions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-transactions-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCTransactions
---
