---
description: ''
layout: schema
name: PreservationProject
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: buildingId
  type: string
- description: ''
  name: buildingName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: estimatedCompletion
  type: string
- description: ''
  name: actualCompletion
  type: string
- description: ''
  name: budget
  type: number
- description: ''
  name: description
  type: string
- description: ''
  name: contractor
  type: string
- description: ''
  name: historicalContext
  type: string
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-preservation-project-schema.json
slug: aoc-data-api-preservation-project
source_filename: aoc-data-api-preservation-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-preservation-project-schema.json\",\n  \"title\": \"PreservationProject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"buildingId\": {\n      \"type\": \"string\"\n    },\n    \"buildingName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"planned\",\n        \"active\",\n        \"completed\"\n      ]\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"estimatedCompletion\": {\n      \"type\": \"string\"\n    },\n    \"actualCompletion\": {\n      \"type\": \"string\"\n    },\n    \"budget\": {\n      \"type\": \"number\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  \n    },\n    \"contractor\": {\n      \"type\": \"string\"\n    },\n    \"historicalContext\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-preservation-project-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: PreservationProject
---
