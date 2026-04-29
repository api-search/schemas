---
description: ''
layout: schema
name: Pricing
properties_list:
- description: The base nightly price in the listing currency.
  name: nightly_price
  type: number
- description: The ISO 4217 currency code for pricing.
  name: currency
  type: string
- description: The one-time cleaning fee charged per reservation.
  name: cleaning_fee
  type: number
- description: The percentage discount for stays of 7 or more nights.
  name: weekly_discount
  type: number
- description: The percentage discount for stays of 28 or more nights.
  name: monthly_discount
  type: number
- description: The additional fee per extra guest beyond the base occupancy.
  name: extra_guest_fee
  type: number
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-pricing-schema.json
slug: airbnb-pricing
source_filename: airbnb-pricing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-pricing-schema.json\",\n  \"title\": \"Pricing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nightly_price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The base nightly price in the listing currency.\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for pricing.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"cleaning_fee\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The one-time cleaning fee charged per reservation.\",\n      \"minimum\": 0\n    },\n    \"weekly_discount\": {\n      \"type\": \"number\",\n      \"description\": \"The percentage discount for stays of 7 or more nights.\",\n      \"minimum\": 0,\n   \
  \   \"maximum\": 100\n    },\n    \"monthly_discount\": {\n      \"type\": \"number\",\n      \"description\": \"The percentage discount for stays of 28 or more nights.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"extra_guest_fee\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The additional fee per extra guest beyond the base occupancy.\",\n      \"minimum\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-pricing-schema.json
tags: []
title: Pricing
---
