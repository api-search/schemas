---
description: a fee
layout: schema
name: Fee
properties_list:
- description: ''
  name: amount
  type: string
- description: ''
  name: type
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-fee-schema.json
slug: flight-choice-prediction-fee
source_filename: flight-choice-prediction-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Fee\",\n  \"description\": \"a fee\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"$ref\": \"#/definitions/FeeType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-fee-schema.json
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
title: Fee
---
