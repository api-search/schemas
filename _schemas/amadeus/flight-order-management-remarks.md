---
description: remarks
layout: schema
name: Remarks
properties_list:
- description: list of general remarks
  name: general
  type: array
- description: list of airline remarks
  name: airline
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-remarks-schema.json
slug: flight-order-management-remarks
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Remarks\",\n  \"description\": \"remarks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"general\": {\n      \"type\": \"array\",\n      \"description\": \"list of general remarks\",\n      \"items\": {\n        \"$ref\": \"#/definitions/GeneralRemark\"\n      }\n    },\n    \"airline\": {\n      \"type\": \"array\",\n      \"description\": \"list of airline remarks\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AirlineRemark\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-remarks-schema.json
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
title: Remarks
---
