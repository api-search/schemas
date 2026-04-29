---
description: PathPoint from Adobe Illustrator API
layout: schema
name: PathPoint
properties_list:
- description: Anchor point coordinates [x, y].
  name: anchor
  type: array
- description: Left control handle coordinates [x, y].
  name: leftDirection
  type: array
- description: Right control handle coordinates [x, y].
  name: rightDirection
  type: array
- description: The type of path point.
  name: pointType
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-path-point-schema.json
slug: adobe-illustrator-scripting-path-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-point-schema.json\",\n  \"title\": \"PathPoint\",\n  \"description\": \"PathPoint from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"anchor\": {\n      \"type\": \"array\",\n      \"description\": \"Anchor point coordinates [x, y].\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"leftDirection\": {\n      \"type\": \"array\",\n      \"description\": \"Left control handle coordinates [x, y].\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"rightDirection\": {\n      \"type\": \"array\",\n      \"description\": \"Right control handle coordinates [x, y].\",\n      \"items\": {\n        \"type\"\
  : \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"pointType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of path point.\",\n      \"enum\": [\n        \"Smooth\",\n        \"Corner\"\n      ],\n      \"example\": \"Smooth\"\n    }\n  },\n  \"required\": [\n    \"anchor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-point-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: PathPoint
---
