---
description: ''
layout: schema
name: response_locationScore
properties_list:
- description: ''
  name: meta
  type: object
- description: ''
  name: data
  type: array
- description: ''
  name: warnings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/location-score-response-locationscore-schema.json
slug: location-score-response-locationscore
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_locationScore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/category-rated-areas\"\n      }\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Warning\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/location-score-response-locationscore-schema.json
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
title: response_locationScore
---
