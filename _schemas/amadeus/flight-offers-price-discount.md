---
description: traveler discount
layout: schema
name: Discount
properties_list:
- description: ''
  name: subType
  type: object
- description: city of residence
  name: cityName
  type: string
- description: ''
  name: travelerType
  type: object
- description: resident card number
  name: cardNumber
  type: string
- description: resident certificate number
  name: certificateNumber
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-discount-schema.json
slug: flight-offers-price-discount
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Discount\",\n  \"description\": \"traveler discount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/DiscountType\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"city of residence\"\n    },\n    \"travelerType\": {\n      \"$ref\": \"#/definitions/DiscountTravelerType\"\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"resident card number\"\n    },\n    \"certificateNumber\": {\n      \"type\": \"string\",\n      \"description\": \"resident certificate number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-discount-schema.json
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
title: Discount
---
