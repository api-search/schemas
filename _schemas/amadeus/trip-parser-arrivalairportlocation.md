---
description: Description of a particular point or place in physical space
layout: schema
name: arrivalAirportLocation
properties_list:
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: ''
  name: address
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-arrivalairportlocation-schema.json
slug: trip-parser-arrivalairportlocation
source_filename: trip-parser-arrivalairportlocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"arrivalAirportLocation\",\n  \"description\": \"Description of a particular point or place in physical space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Label associated to the location (e.g. Eiffel Tower, Madison Square)\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-arrivalairportlocation-schema.json
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
title: arrivalAirportLocation
---
