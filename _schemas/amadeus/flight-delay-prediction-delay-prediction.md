---
description: ''
layout: schema
name: Delay_Prediction
properties_list:
- description: the resource name (`prediction`)
  name: type
  type: string
- description: ''
  name: subType
  type: string
- description: item identifier
  name: id
  type: string
- description: ''
  name: result
  type: object
- description: probability of the forecast (between 0 and 1)
  name: probability
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-delay-prediction-delay-prediction-schema.json
slug: flight-delay-prediction-delay-prediction
source_filename: flight-delay-prediction-delay-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Delay_Prediction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name (`prediction`)\"\n    },\n    \"subType\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"item identifier\"\n    },\n    \"result\": {\n      \"$ref\": \"#/definitions/PredictionResultType\"\n    },\n    \"probability\": {\n      \"type\": \"string\",\n      \"description\": \"probability of the forecast (between 0 and 1)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-delay-prediction-delay-prediction-schema.json
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
title: Delay_Prediction
---
