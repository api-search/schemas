---
description: WarningNotFound schema
layout: schema
name: WarningNotFound
properties_list: []
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-warning-not-found-schema.json
slug: hotel-ratings-warning-not-found
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-warning-not-found-schema.json\",\n  \"title\": \"WarningNotFound\",\n  \"description\": \"WarningNotFound schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Warning\"\n    }\n  ],\n  \"example\": {\n    \"code\": 913,\n    \"title\": \"PROPERTIES NOT FOUND\",\n    \"detail\": \"Some of the requested properties were not found in our database.\",\n    \"source\": {\n      \"parameter\": \"hotelIds\",\n      \"pointer\": \"ABCDEFGH,LPCDEFGQ\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-warning-not-found-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: WarningNotFound
---
