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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-price-schema.json
slug: hotel-booking-price
source_filename: hotel-booking-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-price-schema.json\",\n  \"title\": \"Price\",\n  \"description\": \"Price valuation information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"currency Code apply to all elements of the price\"\n    },\n    \"sellingTotal\": {\n      \"type\": \"string\",\n      \"description\": \"sellingTotal = Total + margins + markup + totalFees - discounts\"\n    },\n    \"total\": {\n      \"type\": \"string\",\n      \"description\": \"total = base + totalTaxes\"\n    },\n    \"base\": {\n      \"type\": \"string\"\n    },\n    \"markups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"Markup\",\n        \"type\": \"object\",\n        \"description\": \"Markup applied to provide a service or\
  \ a product to the client. Typical use case is to convey markup information set by the travel agent.\",\n        \"properties\": {\n          \"amount\": {\n            \"type\": \"string\",\n            \"description\": \"Defines the monetary value with decimal position as a String.\",\n            \"example\": \"10\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-price-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Price
---
