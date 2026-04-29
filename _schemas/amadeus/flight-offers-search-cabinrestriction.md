---
description: ''
layout: schema
name: CabinRestriction
properties_list:
- description: ''
  name: cabin
  type: object
- description: The list of originDestination identifiers for which the cabinRestriction applies
  name: originDestinationIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-cabinrestriction-schema.json
slug: flight-offers-search-cabinrestriction
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CabinRestriction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cabin\": {\n      \"$ref\": \"#/definitions/TravelClass\"\n    },\n    \"originDestinationIds\": {\n      \"type\": \"array\",\n      \"description\": \"The list of originDestination identifiers for which the cabinRestriction applies\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-cabinrestriction-schema.json
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
title: CabinRestriction
---
