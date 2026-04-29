---
description: ''
layout: schema
name: Prediction
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-delay-prediction-prediction-schema.json
slug: flight-delay-prediction-prediction
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Prediction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Delay_Prediction\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Collection_Meta_Link\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-delay-prediction-prediction-schema.json
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
