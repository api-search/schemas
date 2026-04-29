---
description: Geographic coordinates of the hotel.
layout: schema
name: GeoCode
properties_list:
- description: Latitude in decimal degrees.
  name: latitude
  type: number
- description: Longitude in decimal degrees.
  name: longitude
  type: number
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-geo-code-schema.json
slug: hotel-content-geo-code
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-geo-code-schema.json\",\n  \"title\": \"GeoCode\",\n  \"description\": \"Geographic coordinates of the hotel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Latitude in decimal degrees.\",\n      \"example\": 51.508\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Longitude in decimal degrees.\",\n      \"example\": -0.145\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-geo-code-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: GeoCode
---
