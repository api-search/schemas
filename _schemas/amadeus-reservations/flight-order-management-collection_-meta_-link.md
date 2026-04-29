---
description: Collection_Meta_Link schema
layout: schema
name: Collection_Meta_Link
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: links
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-collection_-meta_-link-schema.json
slug: flight-order-management-collection_-meta_-link
source_filename: flight-order-management-collection_-meta_-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-collection_-meta_-link-schema.json\",\n  \"title\": \"Collection_Meta_Link\",\n  \"description\": \"Collection_Meta_Link schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"title\": \"CollectionLinks\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"previous\": {\n          \"type\": \"string\",\n    \
  \      \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"first\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        },\n        \"up\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"example\": \"https://test.api.amadeus.com/v1/area/resources?...\"\n        }\n      },\n      \"example\": {\n        \"self\": \"https://test.api.amadeus.com/v1/area/resources?param=value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-collection_-meta_-link-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Collection_Meta_Link
---
