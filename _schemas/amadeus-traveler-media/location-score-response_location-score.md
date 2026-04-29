---
description: response_locationScore schema
layout: schema
name: response_locationScore
properties_list:
- description: ''
  name: meta
  type: object
- description: ''
  name: data
  type: array
- description: ''
  name: warnings
  type: array
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/location-score-response_location-score-schema.json
slug: location-score-response_location-score
source_filename: location-score-response_location-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/location-score-response_location-score-schema.json\",\n  \"title\": \"response_locationScore\",\n  \"description\": \"response_locationScore schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/Meta\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/category-rated-areas\"\n      }\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Warning\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/location-score-response_location-score-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: response_locationScore
---
