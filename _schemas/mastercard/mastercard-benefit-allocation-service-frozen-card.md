---
description: ''
layout: schema
name: FrozenCard
properties_list:
- description: 16 or 19 digit PAN number that will be frozen/unfrozen.
  name: cardNumber
  type: integer
- description: Date at which the freeze will be effective. Date should be in YYYY-MM-DD format.
  name: date
  type: string
- description: Variable to change whether or not the card number is frozen. True for freeze and false for unfreeze.
  name: isFrozen
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-frozen-card-schema.json
slug: mastercard-benefit-allocation-service-frozen-card
source_filename: mastercard-benefit-allocation-service-frozen-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FrozenCard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"16 or 19 digit PAN number that will be frozen/unfrozen.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date at which the freeze will be effective. Date should be in YYYY-MM-DD format.\"\n    },\n    \"isFrozen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Variable to change whether or not the card number is frozen. True for freeze and false for unfreeze.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-frozen-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: FrozenCard
---
