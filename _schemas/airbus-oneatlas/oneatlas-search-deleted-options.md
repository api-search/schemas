---
description: ''
layout: schema
name: search-deleted-options
properties_list:
- description: The date of items deletions
  name: deletedDate
  type: object
- description: The maximum number of items that the response can contain.
  name: itemsPerPage
  type: integer
- description: The number of skipped items
  name: startIndex
  type: integer
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-search-deleted-options-schema.json
slug: oneatlas-search-deleted-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-deleted-options-schema.json\",\n  \"title\": \"search-deleted-options\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deletedDate\": {\n      \"description\": \"The date of items deletions\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The downloading start date.\",\n          \"example\": \"2017-08-29T00:00:00Z\"\n        },\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time-range\",\n          \"description\": \"The downloading start dates range.\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  -\
  \ Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\\n\",\n          \"example\": \"[2017-08-29T00:00:00Z\"\n        }\n      ]\n    },\n    \"itemsPerPage\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"The maximum number of items that the response can contain.\",\n      \"default\": 50,\n      \"maximum\": 500,\n      \"example\": 100\n    },\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"The number of skipped items\",\n      \"default\": 0,\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-deleted-options-schema.json
tags:
- Imagery
- Satellites
title: search-deleted-options
---
