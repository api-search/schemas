---
description: ''
layout: schema
name: GetFlightOffersQuery
properties_list:
- description: The currency code, as defined in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217), to reflect the currency in which this amount is expressed.
  name: currencyCode
  type: string
- description: 'Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past '
  name: originDestinations
  type: array
- description: 'travelers in the trip. Maximum number of passengers older than 2 yo (CHILD, ADULT, YOUGHT): 9. Each adult can travel with one INFANT so maximum total number of passengers: 18'
  name: travelers
  type: array
- description: Allows enable one or more sources. If present in the list, these sources will be called by the system.
  name: sources
  type: array
- description: ''
  name: searchCriteria
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-getflightoffersquery-schema.json
slug: flight-offers-search-getflightoffersquery
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GetFlightOffersQuery\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code, as defined in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217), to reflect the currency in which this amount is expressed.\"\n    },\n    \"originDestinations\": {\n      \"type\": \"array\",\n      \"description\": \"Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past nor more than 365 days in the future, according to provider settings.Number of Origins and Destinations must not exceed the limit defined in provider settings.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/OriginDestination\"\n      }\n    },\n    \"travelers\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"travelers in the trip. \\n\\n Maximum number of passengers older than 2 yo (CHILD, ADULT, YOUGHT): 9.\\n Each adult can travel with one INFANT so maximum total number of passengers: 18\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_TravelerInfo\"\n      }\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Allows enable one or more sources. If present in the list, these sources will be called by the system.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOfferSource\"\n      }\n    },\n    \"searchCriteria\": {\n      \"$ref\": \"#/definitions/SearchCriteria\"\n    }\n  },\n  \"required\": [\n    \"originDestinations\",\n    \"travelers\",\n    \"sources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-getflightoffersquery-schema.json
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
title: GetFlightOffersQuery
---
