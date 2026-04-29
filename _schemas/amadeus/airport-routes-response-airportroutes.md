---
description: ''
layout: schema
name: response_airportRoutes
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
schema_file: json-schema/airport-routes-response-airportroutes-schema.json
slug: airport-routes-response-airportroutes
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_airportRoutes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/warnings\"\n      }\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/locations\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-routes-response-airportroutes-schema.json
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
title: response_airportRoutes
---
