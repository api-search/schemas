---
description: ''
layout: schema
name: GetFlightAvailabilitiesQuery
properties_list:
- description: 'Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past '
  name: originDestinations
  type: array
- description: List of travelers composing the travel
  name: travelers
  type: array
- description: 'Allows enable one or more sources. If present in the list, these sources will be called by the system. GDS : Full service carriers'
  name: sources
  type: array
- description: ''
  name: searchCriteria
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-getflightavailabilitiesquery-schema.json
slug: flight-availibilities-search-getflightavailabilitiesquery
source_filename: flight-availibilities-search-getflightavailabilitiesquery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GetFlightAvailabilitiesQuery\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"originDestinations\": {\n      \"type\": \"array\",\n      \"description\": \"Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past nor more than 365 days in the future, according to provider settings.Number of Origins and Destinations must not exceed the limit defined in provider settings.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_OriginDestinationLight\"\n      }\n    },\n    \"travelers\": {\n      \"type\": \"array\",\n      \"description\": \"List of travelers composing the travel\",\n      \"items\": {\n        \"$ref\": \"#/definitions/TravelerInfo\"\n      }\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"Allows enable one or more sources. If present in the list, these sources will be called by the system. \\nGDS : Full service carriers\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOfferSource\"\n      }\n    },\n    \"searchCriteria\": {\n      \"$ref\": \"#/definitions/Extended_SearchCriteria\"\n    }\n  },\n  \"required\": [\n    \"originDestinations\",\n    \"travelers\",\n    \"sources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-getflightavailabilitiesquery-schema.json
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
title: GetFlightAvailabilitiesQuery
---
