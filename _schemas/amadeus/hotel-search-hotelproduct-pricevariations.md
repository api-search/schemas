---
description: Daily price variations and the average daily price (when available) is shown here
layout: schema
name: HotelProduct_PriceVariations
properties_list:
- description: ''
  name: average
  type: object
- description: A collection of price periods if the daily price changes during the stay
  name: changes
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-pricevariations-schema.json
slug: hotel-search-hotelproduct-pricevariations
source_filename: hotel-search-hotelproduct-pricevariations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_PriceVariations\",\n  \"description\": \"Daily price variations and the average daily price (when available) is shown here\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"average\": {\n      \"$ref\": \"#/definitions/Price\"\n    },\n    \"changes\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of price periods if the daily price changes during the stay\",\n      \"items\": {\n        \"$ref\": \"#/definitions/HotelProduct_PriceVariation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-pricevariations-schema.json
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
title: HotelProduct_PriceVariations
---
