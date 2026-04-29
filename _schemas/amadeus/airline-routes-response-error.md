---
description: ''
layout: schema
name: response_error
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-response-error-schema.json
slug: airline-routes-response-error
source_filename: airline-routes-response-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/errors\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-routes-response-error-schema.json
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
title: response_error
---
