---
description: Meta information about the returned object(s) in "data"
layout: schema
name: Meta
properties_list:
- description: Total number of object(s) retrieved
  name: count
  type: integer
- description: Links related to the returned object(s)
  name: links
  type: object
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/travel-recommendations-meta-schema.json
slug: travel-recommendations-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-meta-schema.json\",\n  \"title\": \"Meta\",\n  \"description\": \"Meta information about the returned object(s) in \\\"data\\\"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total number of object(s) retrieved\",\n      \"minimum\": 0,\n      \"exclusiveMinimum\": false\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"title\": \"Links\",\n      \"description\": \"Links related to the returned object(s)\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the same page.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-meta-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Meta
---
