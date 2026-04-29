---
description: PathItem from Adobe Illustrator API
layout: schema
name: PathItem
properties_list:
- description: Unique identifier of the path item.
  name: id
  type: string
- description: Name of the path item.
  name: name
  type: string
- description: Whether the path is closed.
  name: closed
  type: boolean
- description: Whether the path has a fill.
  name: filled
  type: boolean
- description: ''
  name: fillColor
  type: object
- description: Whether the path has a stroke.
  name: stroked
  type: boolean
- description: ''
  name: strokeColor
  type: object
- description: Stroke width in points.
  name: strokeWidth
  type: number
- description: Stroke cap style.
  name: strokeCap
  type: string
- description: Stroke join style.
  name: strokeJoin
  type: string
- description: Dash pattern for the stroke.
  name: strokeDashes
  type: array
- description: Opacity as a percentage (0-100).
  name: opacity
  type: number
- description: Blending mode.
  name: blendingMode
  type: string
- description: Position [x, y] in points.
  name: position
  type: array
- description: Width in points.
  name: width
  type: number
- description: Height in points.
  name: height
  type: number
- description: Array of path points defining the path shape.
  name: pathPoints
  type: array
- description: Area of the path in square points.
  name: area
  type: number
- description: Length of the path in points.
  name: length
  type: number
- description: Whether this path item is a guide.
  name: guides
  type: boolean
- description: Whether this path item is a clipping path.
  name: clipping
  type: boolean
- description: Name of the containing layer.
  name: layer
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-path-item-schema.json
slug: adobe-illustrator-scripting-path-item
source_filename: adobe-illustrator-scripting-path-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-item-schema.json\",\n  \"title\": \"PathItem\",\n  \"description\": \"PathItem from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the path item.\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the path item.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"closed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the path is closed.\",\n      \"example\": true\n    },\n    \"filled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the path has a fill.\",\n      \"example\": true\n    },\n    \"fillColor\": {\n      \"$ref\": \"\
  #/components/schemas/Color\"\n    },\n    \"stroked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the path has a stroke.\",\n      \"example\": true\n    },\n    \"strokeColor\": {\n      \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"strokeWidth\": {\n      \"type\": \"number\",\n      \"description\": \"Stroke width in points.\",\n      \"example\": 72.0\n    },\n    \"strokeCap\": {\n      \"type\": \"string\",\n      \"description\": \"Stroke cap style.\",\n      \"enum\": [\n        \"ButtEndCap\",\n        \"RoundEndCap\",\n        \"ProjectingEndCap\"\n      ],\n      \"example\": \"ButtEndCap\"\n    },\n    \"strokeJoin\": {\n      \"type\": \"string\",\n      \"description\": \"Stroke join style.\",\n      \"enum\": [\n        \"MiterEndJoin\",\n        \"RoundEndJoin\",\n        \"BevelEndJoin\"\n      ],\n      \"example\": \"MiterEndJoin\"\n    },\n    \"strokeDashes\": {\n      \"type\": \"array\",\n      \"description\": \"Dash pattern for\
  \ the stroke.\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"opacity\": {\n      \"type\": \"number\",\n      \"description\": \"Opacity as a percentage (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"blendingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Blending mode.\",\n      \"example\": \"example_value\"\n    },\n    \"position\": {\n      \"type\": \"array\",\n      \"description\": \"Position [x, y] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width in points.\",\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height in points.\",\n      \"example\": 72.0\n    },\n    \"pathPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Array of path points defining\
  \ the path shape.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PathPoint\"\n      }\n    },\n    \"area\": {\n      \"type\": \"number\",\n      \"description\": \"Area of the path in square points.\",\n      \"example\": 72.0\n    },\n    \"length\": {\n      \"type\": \"number\",\n      \"description\": \"Length of the path in points.\",\n      \"example\": 72.0\n    },\n    \"guides\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this path item is a guide.\",\n      \"example\": true\n    },\n    \"clipping\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this path item is a clipping path.\",\n      \"example\": true\n    },\n    \"layer\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the containing layer.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-item-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: PathItem
---
