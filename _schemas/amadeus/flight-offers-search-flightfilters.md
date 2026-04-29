---
description: ''
layout: schema
name: FlightFilters
properties_list:
- description: Allows to search a location outside the borders when a radius around a location is specified. Default is false.
  name: crossBorderAllowed
  type: boolean
- description: This flag enables/disables the possibility to have more overnight flights in Low Fare Search
  name: moreOvernightsAllowed
  type: boolean
- description: This option force to retrieve flight-offer with a departure and a return in the same airport
  name: returnToDepartureAirport
  type: boolean
- description: This flag enable/disable filtering of rail segment (TGV AIR, RAIL ...)
  name: railSegmentAllowed
  type: boolean
- description: This flag enable/disable filtering of bus segment
  name: busSegmentAllowed
  type: boolean
- description: Maximum flight time as a percentage relative to the shortest flight time available for the itinerary
  name: maxFlightTime
  type: number
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
schema_file: json-schema/flight-offers-search-flightfilters-schema.json
slug: flight-offers-search-flightfilters
source_filename: flight-offers-search-flightfilters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightFilters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crossBorderAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allows to search a location outside the borders when a radius around a location is specified. Default is false.\"\n    },\n    \"moreOvernightsAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"This flag enables/disables the possibility to have more overnight flights in Low Fare Search\"\n    },\n    \"returnToDepartureAirport\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option force to retrieve flight-offer with a departure and a return in the same airport\"\n    },\n    \"railSegmentAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"This flag enable/disable filtering of rail segment (TGV AIR, RAIL ...)\"\n    },\n    \"busSegmentAllowed\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"This flag enable/disable filtering of bus segment\"\n    },\n    \"maxFlightTime\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum flight time as a percentage relative to the shortest flight time available for the itinerary\"\n    },\n    \"carrierRestrictions\": {\n      \"$ref\": \"#/definitions/CarrierRestrictions\"\n    },\n    \"cabinRestrictions\": {\n      \"type\": \"array\",\n      \"description\": \"Restriction towards cabins.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_CabinRestriction\"\n      }\n    },\n    \"connectionRestriction\": {\n      \"$ref\": \"#/definitions/ConnectionRestriction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-flightfilters-schema.json
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
title: FlightFilters
---
