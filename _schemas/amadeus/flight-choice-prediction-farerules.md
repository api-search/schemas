---
description: ''
layout: schema
name: FareRules
properties_list:
- description: The currency of the penalties
  name: currency
  type: string
- description: ''
  name: rules
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-farerules-schema.json
slug: flight-choice-prediction-farerules
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FareRules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency of the penalties\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/TermAndCondition\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-farerules-schema.json
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
title: FareRules
---
