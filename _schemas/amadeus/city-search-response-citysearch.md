---
description: ''
layout: schema
name: response_citySearch
properties_list:
- description: ''
  name: warnings
  type: array
- description: ''
  name: meta
  type: object
- description: ''
  name: data
  type: array
- description: ''
  name: included
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/city-search-response-citysearch-schema.json
slug: city-search-response-citysearch
source_filename: city-search-response-citysearch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_citySearch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Warning\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Location\"\n      }\n    },\n    \"included\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"airports\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/city-search-response-citysearch-schema.json
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
title: response_citySearch
---
