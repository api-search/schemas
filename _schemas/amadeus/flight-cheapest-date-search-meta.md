---
description: ''
layout: schema
name: Meta
properties_list:
- description: the currency in which the prices of the flight offers are returned. Currency is specified in the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. EUR for Euro
  name: currency
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: defaults
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-cheapest-date-search-meta-schema.json
slug: flight-cheapest-date-search-meta
source_filename: flight-cheapest-date-search-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Meta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"the currency in which the prices of the flight offers are returned. Currency is specified in the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. EUR for Euro\"\n    },\n    \"links\": {\n      \"$ref\": \"#/definitions/Links\"\n    },\n    \"defaults\": {\n      \"$ref\": \"#/definitions/Defaults\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-cheapest-date-search-meta-schema.json
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
title: Meta
---
