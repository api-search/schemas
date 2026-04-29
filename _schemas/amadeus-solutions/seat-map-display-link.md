---
description: Link schema
layout: schema
name: Link
properties_list:
- description: ''
  name: href
  type: string
- description: ''
  name: methods
  type: array
- description: ''
  name: count
  type: integer
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-link-schema.json
slug: seat-map-display-link
source_filename: seat-map-display-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-link-schema.json\",\n  \"title\": \"Link\",\n  \"description\": \"Link schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GET\",\n          \"PUT\",\n          \"DELETE\",\n          \"POST\",\n          \"PATCH\"\n        ]\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"href\"\n  ],\n  \"example\": {\n    \"href\": \"string\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-link-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Link
---
