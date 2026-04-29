---
description: ''
layout: schema
name: marketing
properties_list:
- description: ''
  name: carrier
  type: object
- description: ''
  name: flightDesignator
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-marketing-schema.json
slug: trip-parser-marketing
source_filename: trip-parser-marketing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"marketing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrier\": {\n      \"$ref\": \"#/definitions/carrier\"\n    },\n    \"flightDesignator\": {\n      \"$ref\": \"#/definitions/flightDesignator\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-marketing-schema.json
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
title: marketing
---
