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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-collection_-meta-schema.json
slug: seat-map-display-collection_-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-collection_-meta-schema.json\",\n  \"title\": \"Collection_Meta\",\n  \"description\": \"Collection_Meta schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"title\": \"CollectionLinks\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"previous\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n\
  \          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"first\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"up\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        }\n      },\n      \"example\": {\n        \"self\": \"https://test.api.amadeus.com/v1/area/resources?param=value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-collection_-meta-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Collection_Meta
---
