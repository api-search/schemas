---
description: meta information
layout: schema
name: Collection_Meta
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: links
  type: object
- description: ''
  name: oneWayCombinations
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-collection-meta-schema.json
slug: flight-choice-prediction-collection-meta
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Collection_Meta\",\n  \"description\": \"meta information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"links\": {\n      \"$ref\": \"#/definitions/CollectionLinks\"\n    },\n    \"oneWayCombinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"properties\": {\n          \"originDestinationId\": {\n            \"type\": \"string\"\n          },\n          \"flightOfferIds\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-collection-meta-schema.json
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
title: Collection_Meta
---
