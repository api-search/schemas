---
description: ''
layout: schema
name: Links
properties_list:
- description: ''
  name: href
  type: string
- description: ''
  name: methods
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/points-of-interest-links-schema.json
slug: points-of-interest-links
source_filename: points-of-interest-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Links\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GET\",\n          \"PUT\",\n          \"DELETE\",\n          \"POST\",\n          \"PATCH\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/points-of-interest-links-schema.json
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
title: Links
---
