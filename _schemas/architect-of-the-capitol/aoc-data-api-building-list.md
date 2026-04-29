---
description: ''
layout: schema
name: BuildingList
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
  name: buildings
  type: array
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-building-list-schema.json
slug: aoc-data-api-building-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-building-list-schema.json\",\n  \"title\": \"BuildingList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"buildings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"type\": {},\n          \"yearBuilt\": {},\n          \"architect\": {},\n          \"description\": {},\n          \"address\": {},\n          \"squareFootage\": {},\n          \"floors\": {},\n          \"historicDesignation\": {},\n          \"visitingHours\": {},\n          \"coordinates\": {}\n        }\n      }\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-building-list-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: BuildingList
---
