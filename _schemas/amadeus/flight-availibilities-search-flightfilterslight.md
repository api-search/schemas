---
description: ''
layout: schema
name: FlightFiltersLight
properties_list:
- description: ''
  name: carrierRestrictions
  type: object
- description: Restriction towards cabins.
  name: cabinRestrictions
  type: array
- description: ''
  name: connectionRestriction
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-flightfilterslight-schema.json
slug: flight-availibilities-search-flightfilterslight
source_filename: flight-availibilities-search-flightfilterslight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightFiltersLight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierRestrictions\": {\n      \"$ref\": \"#/definitions/CarrierRestrictions\"\n    },\n    \"cabinRestrictions\": {\n      \"type\": \"array\",\n      \"description\": \"Restriction towards cabins.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/CabinRestriction\"\n      }\n    },\n    \"connectionRestriction\": {\n      \"$ref\": \"#/definitions/ConnectionRestriction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-flightfilterslight-schema.json
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
title: FlightFiltersLight
---
