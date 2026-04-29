---
description: TextFrame from Adobe Illustrator API
layout: schema
name: TextFrame
properties_list:
- description: Unique identifier of the text frame.
  name: id
  type: string
- description: Name of the text frame.
  name: name
  type: string
- description: Type of text frame.
  name: kind
  type: string
- description: The text content of the frame.
  name: contents
  type: string
- description: Position [x, y] in points.
  name: position
  type: array
- description: Width of the text frame in points.
  name: width
  type: number
- description: Height of the text frame in points.
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
- description: Opacity as a percentage (0-100).
  name: opacity
  type: number
- description: Name of the containing layer.
  name: layer
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-text-frame-schema.json
slug: adobe-illustrator-scripting-text-frame
source_filename: adobe-illustrator-scripting-text-frame-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-text-frame-schema.json\",\n  \"title\": \"TextFrame\",\n  \"description\": \"TextFrame from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the text frame.\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the text frame.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Type of text frame.\",\n      \"enum\": [\n        \"PointText\",\n        \"AreaText\",\n        \"PathText\"\n      ],\n      \"example\": \"PointText\"\n    },\n    \"contents\": {\n      \"type\": \"string\",\n      \"description\": \"The text\
  \ content of the frame.\",\n      \"example\": \"example_value\"\n    },\n    \"position\": {\n      \"type\": \"array\",\n      \"description\": \"Position [x, y] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width of the text frame in points.\",\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height of the text frame in points.\",\n      \"example\": 72.0\n    },\n    \"orientation\": {\n      \"type\": \"string\",\n      \"description\": \"Text orientation.\",\n      \"enum\": [\n        \"Horizontal\",\n        \"Vertical\"\n      ],\n      \"example\": \"Horizontal\"\n    },\n    \"characterAttributes\": {\n      \"$ref\": \"#/components/schemas/CharacterAttributes\"\n    },\n    \"paragraphAttributes\": {\n      \"$ref\": \"#/components/schemas/ParagraphAttributes\"\n\
  \    },\n    \"opacity\": {\n      \"type\": \"number\",\n      \"description\": \"Opacity as a percentage (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"layer\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the containing layer.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-text-frame-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: TextFrame
---
