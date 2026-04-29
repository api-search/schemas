---
description: ''
layout: schema
name: response_airlineRoutes
properties_list:
- description: ''
  name: warnings
  type: array
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-response-airlineroutes-schema.json
slug: airline-routes-response-airlineroutes
source_filename: airline-routes-response-airlineroutes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_airlineRoutes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/warnings\"\n      }\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/locations\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-routes-response-airlineroutes-schema.json
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
title: response_airlineRoutes
---
