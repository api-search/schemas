---
description: Collection_Meta schema
layout: schema
name: Collection_Meta
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: links
  type: object
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/points-of-interest-collection_-meta-schema.json
slug: points-of-interest-collection_-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-collection_-meta-schema.json\",\n  \"title\": \"Collection_Meta\",\n  \"description\": \"Collection_Meta schema\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"links\": {\n      \"title\": \"CollectionLinks\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"previous\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\
  \n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"first\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"up\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        }\n      },\n      \"example\": {\n        \"self\": \"https://test.api.amadeus.com/v1/area/resources?param=value\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-collection_-meta-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Collection_Meta
---
