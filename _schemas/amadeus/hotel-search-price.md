---
description: Price valuation information
layout: schema
name: Price
properties_list:
- description: currency Code apply to all elements of the price
  name: currency
  type: string
- description: sellingTotal = Total + margins + markup + totalFees - discounts
  name: sellingTotal
  type: string
- description: total = base + totalTaxes
  name: total
  type: string
- description: ''
  name: base
  type: string
- description: ''
  name: markups
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-price-schema.json
slug: hotel-search-price
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Price\",\n  \"description\": \"Price valuation information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"currency Code apply to all elements of the price\"\n    },\n    \"sellingTotal\": {\n      \"type\": \"string\",\n      \"description\": \"sellingTotal = Total + margins + markup + totalFees - discounts\"\n    },\n    \"total\": {\n      \"type\": \"string\",\n      \"description\": \"total = base + totalTaxes\"\n    },\n    \"base\": {\n      \"type\": \"string\"\n    },\n    \"markups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Markup\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-price-schema.json
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
