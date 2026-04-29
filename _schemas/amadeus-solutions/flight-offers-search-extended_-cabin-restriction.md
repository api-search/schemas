---
description: Extended_CabinRestriction schema
layout: schema
name: Extended_CabinRestriction
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-extended_-cabin-restriction-schema.json
slug: flight-offers-search-extended_-cabin-restriction
source_filename: flight-offers-search-extended_-cabin-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-extended_-cabin-restriction-schema.json\",\n  \"title\": \"Extended_CabinRestriction\",\n  \"description\": \"Extended_CabinRestriction schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/CabinRestriction\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coverage\": {\n          \"$ref\": \"#/definitions/Coverage\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-extended_-cabin-restriction-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Extended_CabinRestriction
---
