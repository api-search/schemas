---
description: Metadata about the response collection.
layout: schema
name: CollectionMeta
properties_list:
- description: Total number of items in the collection.
  name: count
  type: integer
- description: Links related to the collection.
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-collectionmeta-schema.json
slug: airline-code-lookup-collectionmeta
source_filename: airline-code-lookup-collectionmeta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CollectionMeta\",\n  \"description\": \"Metadata about the response collection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items in the collection.\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links related to the collection.\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link to the current request.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-code-lookup-collectionmeta-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: CollectionMeta
---
