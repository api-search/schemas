---
description: FlightFilters schema
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
- description: Restriction towards carriers.
  name: carrierRestrictions
  type: object
- description: Restriction towards cabins.
  name: cabinRestrictions
  type: array
- description: Restriction towards number of connections.
  name: connectionRestriction
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-flight-filters-schema.json
slug: flight-offers-search-flight-filters
source_filename: flight-offers-search-flight-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-flight-filters-schema.json\",\n  \"title\": \"FlightFilters\",\n  \"description\": \"FlightFilters schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crossBorderAllowed\": {\n      \"description\": \"Allows to search a location outside the borders when a radius around a location is specified. Default is false.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"moreOvernightsAllowed\": {\n      \"description\": \"This flag enables/disables the possibility to have more overnight flights in Low Fare Search\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"returnToDepartureAirport\": {\n      \"description\": \"This option force to retrieve flight-offer with a departure and a return in the same airport\",\n      \"type\": \"\
  boolean\",\n      \"example\": false\n    },\n    \"railSegmentAllowed\": {\n      \"description\": \"This flag enable/disable filtering of rail segment (TGV AIR, RAIL ...)\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"busSegmentAllowed\": {\n      \"description\": \"This flag enable/disable filtering of bus segment\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"maxFlightTime\": {\n      \"description\": \"Maximum flight time as a percentage relative to the shortest flight time available for the itinerary\",\n      \"type\": \"number\",\n      \"example\": 200\n    },\n    \"carrierRestrictions\": {\n      \"title\": \"CarrierRestrictions\",\n      \"description\": \"Restriction towards carriers.\",\n      \"$ref\": \"#/definitions/CarrierRestrictions\"\n    },\n    \"cabinRestrictions\": {\n      \"title\": \"CabinRestrictions\",\n      \"description\": \"Restriction towards cabins.\",\n      \"type\": \"array\",\n      \"minItems\"\
  : 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_CabinRestriction\"\n      }\n    },\n    \"connectionRestriction\": {\n      \"title\": \"ConnectionRestriction\",\n      \"description\": \"Restriction towards number of connections.\",\n      \"$ref\": \"#/definitions/ConnectionRestriction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-flight-filters-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FlightFilters
---
