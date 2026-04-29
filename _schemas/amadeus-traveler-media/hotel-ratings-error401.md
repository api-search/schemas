---
description: Error401 schema
layout: schema
name: Error401
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-error401-schema.json
slug: hotel-ratings-error401
source_filename: hotel-ratings-error401-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error401-schema.json\",\n  \"title\": \"Error401\",\n  \"description\": \"Error401 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Error\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 401,\n        \"code\": 20,\n        \"title\": \"RESTRICTED\",\n        \"detail\": \"Query unauthorized\"\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error401-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Error401
---
