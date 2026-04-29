---
description: response_recommendedLocation schema
layout: schema
name: response_recommendedLocation
properties_list:
- description: ''
  name: warnings
  type: array
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/travel-recommendations-response_recommended-location-schema.json
slug: travel-recommendations-response_recommended-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-response_recommended-location-schema.json\",\n  \"title\": \"response_recommendedLocation\",\n  \"description\": \"response_recommendedLocation schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Warning\"\n      }\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RecommendedLocation\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/Meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-response_recommended-location-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: response_recommendedLocation
---
