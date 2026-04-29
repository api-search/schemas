---
description: ''
layout: schema
name: CollectionMeta
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-ratings-collectionmeta-schema.json
slug: hotel-ratings-collectionmeta
source_filename: hotel-ratings-collectionmeta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CollectionMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"links\": {\n      \"$ref\": \"#/definitions/CollectionLinks\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-ratings-collectionmeta-schema.json
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
title: CollectionMeta
---
