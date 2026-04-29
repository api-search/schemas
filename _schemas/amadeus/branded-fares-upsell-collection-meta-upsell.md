---
description: ''
layout: schema
name: Collection_Meta_Upsell
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: oneWayUpselledCombinations
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/branded-fares-upsell-collection-meta-upsell-schema.json
slug: branded-fares-upsell-collection-meta-upsell
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Collection_Meta_Upsell\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"oneWayUpselledCombinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"properties\": {\n          \"flightOfferId\": {\n            \"type\": \"string\"\n          },\n          \"upselledFlightOfferIds\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/branded-fares-upsell-collection-meta-upsell-schema.json
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
title: Collection_Meta_Upsell
---
