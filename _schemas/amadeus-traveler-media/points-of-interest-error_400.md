---
description: Error_400 schema
layout: schema
name: Error_400
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/points-of-interest-error_400-schema.json
slug: points-of-interest-error_400
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-error_400-schema.json\",\n  \"title\": \"Error_400\",\n  \"description\": \"Error_400 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 400,\n        \"code\": 477,\n        \"title\": \"INVALID FORMAT\",\n        \"detail\": \"invalid query parameter format\",\n        \"source\": {\n          \"parameter\": \"airport\",\n          \"example\": \"CDG\"\n        }\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-error_400-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Error_400
---
