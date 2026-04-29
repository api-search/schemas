---
description: This object holds the transaction footprint for a payment transaction.
layout: schema
name: MCTransactionFootprint
properties_list:
- description: The transaction's CO2 emission in grams
  name: carbonEmissionInGrams
  type: number
- description: The transaction's CO2 emission in ounces
  name: carbonEmissionInOunces
  type: number
- description: The transaction's CO2 emission cost
  name: carbonSocialCost
  type: object
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-transaction-footprint-schema.json
slug: mastercard-doconomy-aland-index-mc-transaction-footprint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCTransactionFootprint\",\n  \"type\": \"object\",\n  \"description\": \"This object holds the transaction footprint for a payment transaction.\",\n  \"properties\": {\n    \"carbonEmissionInGrams\": {\n      \"type\": \"number\",\n      \"description\": \"The transaction's CO2 emission in grams\"\n    },\n    \"carbonEmissionInOunces\": {\n      \"type\": \"number\",\n      \"description\": \"The transaction's CO2 emission in ounces\"\n    },\n    \"carbonSocialCost\": {\n      \"type\": \"object\",\n      \"description\": \"The transaction's CO2 emission cost\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-transaction-footprint-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCTransactionFootprint
---
