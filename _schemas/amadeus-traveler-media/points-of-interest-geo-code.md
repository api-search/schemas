---
description: GeoCode schema
layout: schema
name: GeoCode
properties_list:
- description: latitude of the location
  name: latitude
  type: number
- description: longitude of the location
  name: longitude
  type: number
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/points-of-interest-geo-code-schema.json
slug: points-of-interest-geo-code
source_filename: points-of-interest-geo-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-geo-code-schema.json\",\n  \"title\": \"GeoCode\",\n  \"description\": \"GeoCode schema\",\n  \"properties\": {\n    \"latitude\": {\n      \"description\": \"latitude of the location\",\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"example\": 43.580418\n    },\n    \"longitude\": {\n      \"description\": \"longitude of the location\",\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"example\": 7.125102\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-geo-code-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: GeoCode
---
