---
description: Collection_Meta_Upsell schema
layout: schema
name: Collection_Meta_Upsell
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: oneWayUpselledCombinations
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-collection_-meta_-upsell-schema.json
slug: branded-fares-upsell-collection_-meta_-upsell
source_filename: branded-fares-upsell-collection_-meta_-upsell-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-collection_-meta_-upsell-schema.json\",\n  \"title\": \"Collection_Meta_Upsell\",\n  \"description\": \"Collection_Meta_Upsell schema\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"oneWayUpselledCombinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"oneWayUpselledCombinations\",\n        \"properties\": {\n          \"flightOfferId\": {\n            \"type\": \"string\"\n          },\n          \"upselledFlightOfferIds\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-collection_-meta_-upsell-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Collection_Meta_Upsell
---
