---
description: Response containing hotel content data for one or more hotels.
layout: schema
name: HotelContentResponse
properties_list:
- description: Array of hotel content objects.
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-content-response-schema.json
slug: hotel-content-hotel-content-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-content-response-schema.json\",\n  \"title\": \"HotelContentResponse\",\n  \"description\": \"Response containing hotel content data for one or more hotels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of hotel content objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HotelContent\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/Meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-content-response-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelContentResponse
---
