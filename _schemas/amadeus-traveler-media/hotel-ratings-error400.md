---
description: Error400 schema
layout: schema
name: Error400
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-error400-schema.json
slug: hotel-ratings-error400
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error400-schema.json\",\n  \"title\": \"Error400\",\n  \"description\": \"Error400 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Error\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error400-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Error400
---
