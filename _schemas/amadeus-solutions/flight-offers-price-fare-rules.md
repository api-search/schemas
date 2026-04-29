---
description: FareRules schema
layout: schema
name: FareRules
properties_list:
- description: The currency of the penalties
  name: currency
  type: string
- description: ''
  name: rules
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-fare-rules-schema.json
slug: flight-offers-price-fare-rules
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-fare-rules-schema.json\",\n  \"title\": \"FareRules\",\n  \"description\": \"FareRules schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency of the penalties\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/definitions/TermAndCondition\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-fare-rules-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FareRules
---
