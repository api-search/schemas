---
description: ''
layout: schema
name: response_recommendedLocation
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
schema_file: json-schema/travel-recommendations-response-recommendedlocation-schema.json
slug: travel-recommendations-response-recommendedlocation
source_filename: travel-recommendations-response-recommendedlocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_recommendedLocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Warning\"\n      }\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/RecommendedLocation\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/travel-recommendations-response-recommendedlocation-schema.json
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
title: response_recommendedLocation
---
