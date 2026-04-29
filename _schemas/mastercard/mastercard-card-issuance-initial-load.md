---
description: ''
layout: schema
name: InitialLoad
properties_list:
- description: The currency in which the amount is loaded. <br/> **Valid values :** 3-letter currency codes in `ISO 4217`
  name: currency
  type: string
- description: The amount that can be loaded to the client account.
  name: amount
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-initial-load-schema.json
slug: mastercard-card-issuance-initial-load
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitialLoad\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency in which the amount is loaded. <br/> **Valid values :** 3-letter currency codes in `ISO 4217`\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The amount that can be loaded to the client account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-initial-load-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: InitialLoad
---
