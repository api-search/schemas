---
description: ''
layout: schema
name: DetailedFareRules
properties_list:
- description: ''
  name: fareBasis
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: fareNotes
  type: object
- description: Id of the segment concerned by the fare rule
  name: segmentId
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-detailedfarerules-schema.json
slug: flight-offers-price-detailedfarerules
source_filename: flight-offers-price-detailedfarerules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DetailedFareRules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fareBasis\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"fareNotes\": {\n      \"$ref\": \"#/definitions/TermAndCondition\"\n    },\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the segment concerned by the fare rule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-detailedfarerules-schema.json
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
title: DetailedFareRules
---
