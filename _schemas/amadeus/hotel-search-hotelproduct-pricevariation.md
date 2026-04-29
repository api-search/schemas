---
description: Some prices may vary during a stay, thus here you can see the daily price per period of the stay
layout: schema
name: HotelProduct_PriceVariation
properties_list:
- description: 'Begin date of the period Format: YYYY-MM-DD'
  name: startDate
  type: string
- description: 'End date of the period Format: YYYY-MM-DD'
  name: endDate
  type: string
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
schema_file: json-schema/hotel-search-hotelproduct-pricevariation-schema.json
slug: hotel-search-hotelproduct-pricevariation
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_PriceVariation\",\n  \"description\": \"Some prices may vary during a stay, thus here you can see the daily price per period of the stay\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Begin date of the period\\nFormat: YYYY-MM-DD\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the period\\nFormat: YYYY-MM-DD\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"currency Code apply to all elements of the price\"\n    },\n    \"sellingTotal\": {\n      \"type\": \"string\",\n      \"description\": \"sellingTotal = Total + margins + markup + totalFees - discounts\"\n    },\n    \"total\": {\n      \"type\": \"string\",\n      \"description\": \"total = base + totalTaxes\"\n\
  \    },\n    \"base\": {\n      \"type\": \"string\"\n    },\n    \"markups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Markup\"\n      }\n    }\n  },\n  \"required\": [\n    \"startDate\",\n    \"endDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-pricevariation-schema.json
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
title: HotelProduct_PriceVariation
---
