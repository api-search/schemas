---
description: departure or arrival information
layout: schema
name: OriginalFlightEndPoint
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: terminal name / number
  name: terminal
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-originalflightendpoint-schema.json
slug: flight-offers-price-originalflightendpoint
source_filename: flight-offers-price-originalflightendpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OriginalFlightEndPoint\",\n  \"description\": \"departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\"\n    },\n    \"terminal\": {\n      \"type\": \"string\",\n      \"description\": \"terminal name / number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-originalflightendpoint-schema.json
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
title: OriginalFlightEndPoint
---
