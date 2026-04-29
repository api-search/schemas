---
description: ''
layout: schema
name: AccountDetails
properties_list:
- description: Unique identifier for the Primary Account Number of the card.
  name: accountNumber
  type: string
- description: The last four digits of the card number.
  name: cardLast4
  type: string
- description: The expiry year and month of the card in YYMM format.
  name: cardExpiryDate
  type: string
- description: The first digits of the card number.
  name: cardBin
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-account-details-schema.json
slug: mastercard-identity-insights-for-transactions-account-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Primary Account Number of the card.\"\n    },\n    \"cardLast4\": {\n      \"type\": \"string\",\n      \"description\": \"The last four digits of the card number.\"\n    },\n    \"cardExpiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"The expiry year and month of the card in YYMM format.\"\n    },\n    \"cardBin\": {\n      \"type\": \"string\",\n      \"description\": \"The first digits of the card number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-account-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AccountDetails
---
