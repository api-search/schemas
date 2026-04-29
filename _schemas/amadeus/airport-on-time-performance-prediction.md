---
description: ''
layout: schema
name: Prediction
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: meta
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-on-time-performance-prediction-schema.json
slug: airport-on-time-performance-prediction
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Prediction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/definitions/OnTimePrediction\"\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-on-time-performance-prediction-schema.json
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
title: Prediction
---
