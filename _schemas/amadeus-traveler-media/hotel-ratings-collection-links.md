---
description: CollectionLinks schema
layout: schema
name: CollectionLinks
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: next
  type: string
- description: ''
  name: previous
  type: string
- description: ''
  name: last
  type: string
- description: ''
  name: first
  type: string
- description: ''
  name: up
  type: string
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-collection-links-schema.json
slug: hotel-ratings-collection-links
source_filename: hotel-ratings-collection-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-collection-links-schema.json\",\n  \"title\": \"CollectionLinks\",\n  \"description\": \"CollectionLinks schema\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    },\n    \"last\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    },\n    \"first\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    },\n    \"up\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n    }\n  },\n  \"example\": {\n    \"self\": \"https://test.api.amadeus.com/v1/area/resources?param=value\"\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-collection-links-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: CollectionLinks
---
