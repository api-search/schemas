---
description: Error_500 schema
layout: schema
name: Error_500
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/points-of-interest-error_500-schema.json
slug: points-of-interest-error_500
source_filename: points-of-interest-error_500-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-error_500-schema.json\",\n  \"title\": \"Error_500\",\n  \"description\": \"Error_500 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 500,\n        \"code\": 141,\n        \"title\": \"SYSTEM ERROR HAS OCCURRED\"\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-error_500-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Error_500
---
