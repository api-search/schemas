---
description: DetailedFareRules schema
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-detailed-fare-rules-schema.json
slug: flight-offers-price-detailed-fare-rules
source_filename: flight-offers-price-detailed-fare-rules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-detailed-fare-rules-schema.json\",\n  \"title\": \"DetailedFareRules\",\n  \"description\": \"DetailedFareRules schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fareBasis\": {\n      \"type\": \"string\",\n      \"example\": \"VRDFR9\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"fareNotes\": {\n      \"$ref\": \"#/definitions/TermAndCondition\"\n    },\n    \"segmentId\": {\n      \"description\": \"Id of the segment concerned by the fare rule\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-detailed-fare-rules-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: DetailedFareRules
---
