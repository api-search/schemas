---
description: ''
layout: schema
name: ArtworkList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: artworks
  type: array
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-artwork-list-schema.json
slug: aoc-data-api-artwork-list
source_filename: aoc-data-api-artwork-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-artwork-list-schema.json\",\n  \"title\": \"ArtworkList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"artworks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"title\": {},\n          \"artist\": {},\n          \"yearCreated\": {},\n          \"medium\": {},\n          \"dimensions\": {},\n          \"location\": {},\n          \"buildingId\": {},\n          \"description\": {},\n          \"imageUrl\": {},\n          \"acquisitionDate\": {},\n          \"historicalSignificance\": {}\n        }\n      }\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-artwork-list-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: ArtworkList
---
