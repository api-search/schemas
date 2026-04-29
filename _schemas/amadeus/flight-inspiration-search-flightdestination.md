---
description: ''
layout: schema
name: FlightDestination
properties_list:
- description: the resource name
  name: type
  type: string
- description: ''
  name: origin
  type: string
- description: ''
  name: destination
  type: string
- description: ''
  name: departureDate
  type: string
- description: ''
  name: returnDate
  type: string
- description: ''
  name: price
  type: object
- description: ''
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-inspiration-search-flightdestination-schema.json
slug: flight-inspiration-search-flightdestination
source_filename: flight-inspiration-search-flightdestination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"origin\": {\n      \"type\": \"string\"\n    },\n    \"destination\": {\n      \"type\": \"string\"\n    },\n    \"departureDate\": {\n      \"type\": \"string\"\n    },\n    \"returnDate\": {\n      \"type\": \"string\"\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/Price\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"flightDates\": {\n          \"type\": \"string\"\n        },\n        \"flightOffers\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-inspiration-search-flightdestination-schema.json
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
title: FlightDestination
---
