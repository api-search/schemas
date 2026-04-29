---
description: StringCollectionContract schema from AeroDataBox API
layout: schema
name: StringCollectionContract
properties_list:
- description: The number of items in the collection
  name: count
  type: integer
- description: The collection of items
  name: items
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-string-collection-contract-schema.json
slug: aerodatabox-string-collection-contract
source_filename: aerodatabox-string-collection-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-string-collection-contract-schema.json\",\n  \"title\": \"StringCollectionContract\",\n  \"description\": \"StringCollectionContract schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the collection\",\n      \"format\": \"int32\",\n      \"readOnly\": true\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The collection of items\"\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"items\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-string-collection-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: StringCollectionContract
---
