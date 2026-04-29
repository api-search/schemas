---
description: ''
layout: schema
name: PreservationProjectList
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
  name: projects
  type: array
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-preservation-project-list-schema.json
slug: aoc-data-api-preservation-project-list
source_filename: aoc-data-api-preservation-project-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-preservation-project-list-schema.json\",\n  \"title\": \"PreservationProjectList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"buildingId\": {},\n          \"buildingName\": {},\n          \"status\": {},\n          \"startDate\": {},\n          \"estimatedCompletion\": {},\n          \"actualCompletion\": {},\n          \"budget\": {},\n          \"description\": {},\n          \"contractor\": {},\n          \"historicalContext\"\
  : {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-preservation-project-list-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: PreservationProjectList
---
