---
description: A debit or credit card linked to a customer account
layout: schema
name: Card
properties_list:
- description: Unique card identifier
  name: cardId
  type: string
- description: Masked card number
  name: cardNumber
  type: string
- description: Type of card
  name: cardType
  type: string
- description: Linked account identifier
  name: accountId
  type: string
- description: Card holder customer identifier
  name: customerId
  type: string
- description: Name on the card
  name: cardholderName
  type: string
- description: Card expiry date (MM/YY)
  name: expiryDate
  type: string
- description: Card status
  name: status
  type: string
- description: Daily transaction limit
  name: dailyLimit
  type: number
- description: Available spending limit
  name: availableLimit
  type: number
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-card-schema.json
slug: temenos-transact-core-banking-card
source_filename: temenos-transact-core-banking-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Card\",\n  \"type\": \"object\",\n  \"description\": \"A debit or credit card linked to a customer account\",\n  \"properties\": {\n    \"cardId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique card identifier\"\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Masked card number\"\n    },\n    \"cardType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of card\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Linked account identifier\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Card holder customer identifier\"\n    },\n    \"cardholderName\": {\n      \"type\": \"string\",\n      \"description\": \"Name on the card\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Card expiry date (MM/YY)\"\n    },\n   \
  \ \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Card status\"\n    },\n    \"dailyLimit\": {\n      \"type\": \"number\",\n      \"description\": \"Daily transaction limit\"\n    },\n    \"availableLimit\": {\n      \"type\": \"number\",\n      \"description\": \"Available spending limit\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-card-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Card
---
