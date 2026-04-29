---
description: Amount object that includes the value and the currency in which a payment transaction has been performed
layout: schema
name: MCAmount
properties_list:
- description: Actual amount of a payment transaction
  name: value
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-amount-schema.json
slug: mastercard-doconomy-aland-index-mc-amount
source_filename: mastercard-doconomy-aland-index-mc-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCAmount\",\n  \"type\": \"object\",\n  \"description\": \"Amount object that includes the value and the currency in which a payment transaction has been performed\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Actual amount of a payment transaction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-amount-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCAmount
---
