---
description: This object represents one merchant category information.
layout: schema
name: MCMerchantCategory
properties_list:
- description: Merchant category code of a payment transaction that uniquely defines a merchant business.
  name: mcc
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-merchant-category-schema.json
slug: mastercard-doconomy-aland-index-mc-merchant-category
source_filename: mastercard-doconomy-aland-index-mc-merchant-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCMerchantCategory\",\n  \"type\": \"object\",\n  \"description\": \"This object represents one merchant category information.\",\n  \"properties\": {\n    \"mcc\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant category code of a payment transaction that uniquely defines a merchant business.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-merchant-category-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCMerchantCategory
---
