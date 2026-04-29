---
description: GetFlightOffersQuery schema
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-get-flight-offers-query-schema.json
slug: flight-offers-search-get-flight-offers-query
source_filename: flight-offers-search-get-flight-offers-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-get-flight-offers-query-schema.json\",\n  \"title\": \"GetFlightOffersQuery\",\n  \"description\": \"GetFlightOffersQuery schema\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code, as defined in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217), to reflect the currency in which this amount is expressed.\",\n      \"example\": \"EUR\"\n    },\n    \"originDestinations\": {\n      \"title\": \"originDestinations\",\n      \"description\": \"Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past nor more than 365 days in the future, according to provider settings.Number\
  \ of Origins and Destinations must not exceed the limit defined in provider settings.\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/OriginDestination\"\n      }\n    },\n    \"travelers\": {\n      \"title\": \"travelers\",\n      \"description\": \"travelers in the trip. \\n\\n Maximum number of passengers older than 2 yo (CHILD, ADULT, YOUGHT): 9.\\n Each adult can travel with one INFANT so maximum total number of passengers: 18\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 18,\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_TravelerInfo\"\n      }\n    },\n    \"sources\": {\n      \"title\": \"sources\",\n      \"description\": \"Allows enable one or more sources. If present in the list, these sources will be called by the system.\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOfferSource\"\
  \n      }\n    },\n    \"searchCriteria\": {\n      \"$ref\": \"#/definitions/SearchCriteria\"\n    }\n  },\n  \"required\": [\n    \"originDestinations\",\n    \"travelers\",\n    \"sources\"\n  ],\n  \"example\": {\n    \"currencyCode\": \"USD\",\n    \"originDestinations\": [\n      {\n        \"id\": \"1\",\n        \"originLocationCode\": \"NYC\",\n        \"destinationLocationCode\": \"MAD\",\n        \"departureDateTimeRange\": {\n          \"date\": \"2023-11-01\",\n          \"time\": \"10:00:00\"\n        }\n      }\n    ],\n    \"travelers\": [\n      {\n        \"id\": \"1\",\n        \"travelerType\": \"ADULT\"\n      }\n    ],\n    \"sources\": [\n      \"GDS\"\n    ],\n    \"searchCriteria\": {\n      \"maxFlightOffers\": 2,\n      \"flightFilters\": {\n        \"cabinRestrictions\": [\n          {\n            \"cabin\": \"BUSINESS\",\n            \"coverage\": \"MOST_SEGMENTS\",\n            \"originDestinationIds\": [\n              \"1\"\n            ]\n          }\n\
  \        ]\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-get-flight-offers-query-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: GetFlightOffersQuery
---
