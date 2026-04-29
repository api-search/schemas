---
description: ''
layout: schema
name: HotelProduct_Commission
properties_list:
- description: Percentage of the commission paid to the travel seller. Value is between 0 and 100
  name: percentage
  type: string
- description: Amount of the commission paid to the travel seller. The amount is always linked to the currency code of the offer
  name: amount
  type: string
- description: ''
  name: description
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-commission-schema.json
slug: hotel-search-hotelproduct-commission
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_Commission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the commission paid to the travel seller. Value is between 0 and 100\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of the commission paid to the travel seller. The amount is always linked to the currency code of the offer\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-commission-schema.json
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
title: HotelProduct_Commission
---
