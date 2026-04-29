---
description: ''
layout: schema
name: Link
properties_list:
- description: ''
  name: href
  type: string
- description: ''
  name: methods
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/tours-and-activities-link-schema.json
slug: tours-and-activities-link
source_filename: tours-and-activities-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Link\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GET\",\n          \"PUT\",\n          \"DELETE\",\n          \"POST\",\n          \"PATCH\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/tours-and-activities-link-schema.json
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
title: Link
---
