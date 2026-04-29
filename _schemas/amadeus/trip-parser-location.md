---
description: Description of a particular point or place in physical space
layout: schema
name: location
properties_list:
- description: IATA location code
  name: iataCode
  type: string
- description: ''
  name: address
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-location-schema.json
slug: trip-parser-location
source_filename: trip-parser-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"location\",\n  \"description\": \"Description of a particular point or place in physical space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA location code\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-location-schema.json
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
title: location
---
