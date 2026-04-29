---
description: Meta information about the returned object(s) in "data"
layout: schema
name: Meta
properties_list:
- description: Total number of object(s) retrieved
  name: count
  type: integer
- description: Links related to the returned object(s)
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/city-search-meta-schema.json
slug: city-search-meta
source_filename: city-search-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Meta\",\n  \"description\": \"Meta information about the returned object(s) in \\\"data\\\"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total number of object(s) retrieved\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links related to the returned object(s)\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the same page.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/city-search-meta-schema.json
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
