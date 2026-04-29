---
description: ''
layout: schema
name: Price
properties_list:
- description: ''
  name: currency
  type: string
- description: Total amount paid by the user
  name: total
  type: string
- description: Amount without taxes
  name: base
  type: string
- description: List of applicable fees
  name: fees
  type: array
- description: ''
  name: taxes
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-price-schema.json
slug: flight-choice-prediction-price
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Price\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"total\": {\n      \"type\": \"string\",\n      \"description\": \"Total amount paid by the user\"\n    },\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Amount without taxes\"\n    },\n    \"fees\": {\n      \"type\": \"array\",\n      \"description\": \"List of applicable fees\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Fee\"\n      }\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Tax\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-price-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Price
---
