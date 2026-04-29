---
description: Meta information about the returned object(s) in "data"
layout: schema
name: meta
properties_list:
- description: Total number of object(s) retrieved
  name: count
  type: integer
- description: Links related to the returned object(s)
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-meta-schema.json
slug: airline-routes-meta
source_filename: airline-routes-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"meta\",\n  \"description\": \"Meta information about the returned object(s) in \\\"data\\\"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total number of object(s) retrieved\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links related to the returned object(s)\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link to the same page.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-routes-meta-schema.json
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
title: meta
---
