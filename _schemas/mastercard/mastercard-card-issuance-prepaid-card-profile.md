---
description: ''
layout: schema
name: PrepaidCardProfile
properties_list:
- description: Echo back the branchCode.
  name: branchCode
  type: string
- description: List of cards.
  name: cards
  type: array
- description: List of accounts linked to the card returned
  name: accounts
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-prepaid-card-profile-schema.json
slug: mastercard-card-issuance-prepaid-card-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrepaidCardProfile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchCode\": {\n      \"type\": \"string\",\n      \"description\": \"Echo back the branchCode.\"\n    },\n    \"cards\": {\n      \"type\": \"array\",\n      \"description\": \"List of cards.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts linked to the card returned\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-prepaid-card-profile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PrepaidCardProfile
---
