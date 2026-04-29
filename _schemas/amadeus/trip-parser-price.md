---
description: Price valuation information
layout: schema
name: price
properties_list:
- description: currency Code apply to all elements of the price
  name: currency
  type: string
- description: Total = base + totalTaxes +
  name: total
  type: string
- description: ''
  name: base
  type: string
- description: ''
  name: totalTaxes
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-price-schema.json
slug: trip-parser-price
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"price\",\n  \"description\": \"Price valuation information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"currency Code apply to all elements of the price\"\n    },\n    \"total\": {\n      \"type\": \"string\",\n      \"description\": \"Total = base + totalTaxes +\"\n    },\n    \"base\": {\n      \"type\": \"string\"\n    },\n    \"totalTaxes\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-price-schema.json
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
title: price
---
