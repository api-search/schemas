---
description: CabinRestriction schema
layout: schema
name: CabinRestriction
properties_list:
- description: ''
  name: cabin
  type: object
- description: The list of originDestination identifiers for which the cabinRestriction applies
  name: originDestinationIds
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-cabin-restriction-schema.json
slug: flight-offers-search-cabin-restriction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-cabin-restriction-schema.json\",\n  \"title\": \"CabinRestriction\",\n  \"description\": \"CabinRestriction schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cabin\": {\n      \"$ref\": \"#/definitions/TravelClass\"\n    },\n    \"originDestinationIds\": {\n      \"title\": \"originDestinationIds\",\n      \"description\": \"The list of originDestination identifiers for which the cabinRestriction applies\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        1,\n        2\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-cabin-restriction-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: CabinRestriction
---
