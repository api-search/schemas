---
description: ''
layout: schema
name: AccessibilityInfo
properties_list:
- description: ''
  name: buildingId
  type: string
- description: ''
  name: buildingName
  type: string
- description: ''
  name: wheelchairAccess
  type: boolean
- description: ''
  name: accessibleEntrances
  type: array
- description: ''
  name: elevators
  type: boolean
- description: ''
  name: accessibleRestrooms
  type: boolean
- description: ''
  name: assistiveListeningDevices
  type: boolean
- description: ''
  name: signLanguageInterpretation
  type: string
- description: ''
  name: accessibilityContactPhone
  type: string
- description: ''
  name: notes
  type: string
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-accessibility-info-schema.json
slug: aoc-data-api-accessibility-info
source_filename: aoc-data-api-accessibility-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-accessibility-info-schema.json\",\n  \"title\": \"AccessibilityInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buildingId\": {\n      \"type\": \"string\"\n    },\n    \"buildingName\": {\n      \"type\": \"string\"\n    },\n    \"wheelchairAccess\": {\n      \"type\": \"boolean\"\n    },\n    \"accessibleEntrances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"elevators\": {\n      \"type\": \"boolean\"\n    },\n    \"accessibleRestrooms\": {\n      \"type\": \"boolean\"\n    },\n    \"assistiveListeningDevices\": {\n      \"type\": \"boolean\"\n    },\n    \"signLanguageInterpretation\": {\n      \"type\": \"string\"\n    },\n    \"accessibilityContactPhone\": {\n      \"type\": \"string\"\n    },\n    \"notes\"\
  : {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-accessibility-info-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: AccessibilityInfo
---
