---
description: Collection_Meta schema
layout: schema
name: Collection_Meta
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: oneWayCombinations
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-collection_-meta-schema.json
slug: flight-offers-search-collection_-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-collection_-meta-schema.json\",\n  \"title\": \"Collection_Meta\",\n  \"description\": \"Collection_Meta schema\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"oneWayCombinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"oneWayCombinations\",\n        \"properties\": {\n          \"originDestinationId\": {\n            \"type\": \"string\"\n          },\n          \"flightOfferIds\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-collection_-meta-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Collection_Meta
---
