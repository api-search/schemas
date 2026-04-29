---
description: ''
layout: schema
name: CardExpiry
properties_list:
- description: Denotes a month by when the card will be expired.
  name: month
  type: string
- description: Denotes a year by when the card will be expired.
  name: year
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-card-expiry-schema.json
slug: mastercard-carbon-calculator-experience-card-expiry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CardExpiry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"month\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes a month by when the card will be expired.\"\n    },\n    \"year\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes a year by when the card will be expired.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-card-expiry-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CardExpiry
---
