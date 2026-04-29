---
description: ''
layout: schema
name: FlightDates
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: dictionaries
  type: object
- description: ''
  name: meta
  type: object
- description: ''
  name: warnings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-cheapest-date-search-flightdates-schema.json
slug: flight-cheapest-date-search-flightdates
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightDates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightDate\"\n      }\n    },\n    \"dictionaries\": {\n      \"$ref\": \"#/definitions/Dictionaries\"\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-cheapest-date-search-flightdates-schema.json
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
title: FlightDates
---
