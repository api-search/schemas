---
description: TextFrameCreate from Adobe Illustrator API
layout: schema
name: TextFrameCreate
properties_list:
- description: Name of the text frame.
  name: name
  type: string
- description: Type of text frame to create.
  name: kind
  type: string
- description: The text content.
  name: contents
  type: string
- description: Position [x, y] in points.
  name: position
  type: array
- description: Width for area text frames.
  name: width
  type: number
- description: Height for area text frames.
  name: height
  type: number
- description: Text orientation.
  name: orientation
  type: string
- description: ''
  name: characterAttributes
  type: object
- description: ''
  name: paragraphAttributes
  type: object
- description: Target layer name.
  name: layer
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-text-frame-create-schema.json
slug: adobe-illustrator-scripting-text-frame-create
source_filename: adobe-illustrator-scripting-text-frame-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-text-frame-create-schema.json\",\n  \"title\": \"TextFrameCreate\",\n  \"description\": \"TextFrameCreate from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the text frame.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Type of text frame to create.\",\n      \"enum\": [\n        \"PointText\",\n        \"AreaText\",\n        \"PathText\"\n      ],\n      \"default\": \"PointText\",\n      \"example\": \"PointText\"\n    },\n    \"contents\": {\n      \"type\": \"string\",\n      \"description\": \"The text content.\",\n      \"example\": \"example_value\"\n    },\n    \"position\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Position [x, y] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width for area text frames.\",\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height for area text frames.\",\n      \"example\": 72.0\n    },\n    \"orientation\": {\n      \"type\": \"string\",\n      \"description\": \"Text orientation.\",\n      \"enum\": [\n        \"Horizontal\",\n        \"Vertical\"\n      ],\n      \"default\": \"Horizontal\",\n      \"example\": \"Horizontal\"\n    },\n    \"characterAttributes\": {\n      \"$ref\": \"#/components/schemas/CharacterAttributes\"\n    },\n    \"paragraphAttributes\": {\n      \"$ref\": \"#/components/schemas/ParagraphAttributes\"\n    },\n    \"layer\": {\n      \"type\": \"string\",\n      \"description\": \"Target\
  \ layer name.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"contents\",\n    \"position\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-text-frame-create-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: TextFrameCreate
---
