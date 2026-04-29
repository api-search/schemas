---
description: PathItemCreate from Adobe Illustrator API
layout: schema
name: PathItemCreate
properties_list:
- description: Name of the path item.
  name: name
  type: string
- description: Type of path to create.
  name: pathType
  type: string
- description: Array of path points for freeform paths. Required when pathType is "freeform".
  name: pathPoints
  type: array
- description: Position [x, y] in points.
  name: position
  type: array
- description: Width in points (for rectangle, ellipse).
  name: width
  type: number
- description: Height in points (for rectangle, ellipse).
  name: height
  type: number
- description: Corner radius for rounded rectangle.
  name: cornerRadius
  type: number
- description: Number of sides for polygon.
  name: sides
  type: integer
- description: Number of points for star.
  name: points
  type: integer
- description: Inner radius for star.
  name: innerRadius
  type: number
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
- description: Opacity as a percentage (0-100).
  name: opacity
  type: number
- description: Target layer name.
  name: layer
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-path-item-create-schema.json
slug: adobe-illustrator-scripting-path-item-create
source_filename: adobe-illustrator-scripting-path-item-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-item-create-schema.json\",\n  \"title\": \"PathItemCreate\",\n  \"description\": \"PathItemCreate from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the path item.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"pathType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of path to create.\",\n      \"enum\": [\n        \"freeform\",\n        \"rectangle\",\n        \"roundedRectangle\",\n        \"ellipse\",\n        \"polygon\",\n        \"star\",\n        \"line\"\n      ],\n      \"default\": \"freeform\",\n      \"example\": \"freeform\"\n    },\n    \"pathPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Array of path\
  \ points for freeform paths. Required when pathType is \\\"freeform\\\".\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PathPoint\"\n      }\n    },\n    \"position\": {\n      \"type\": \"array\",\n      \"description\": \"Position [x, y] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width in points (for rectangle, ellipse).\",\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height in points (for rectangle, ellipse).\",\n      \"example\": 72.0\n    },\n    \"cornerRadius\": {\n      \"type\": \"number\",\n      \"description\": \"Corner radius for rounded rectangle.\",\n      \"example\": 72.0\n    },\n    \"sides\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of sides for polygon.\",\n      \"minimum\": 3,\n      \"example\": 1024\n\
  \    },\n    \"points\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of points for star.\",\n      \"minimum\": 3,\n      \"example\": 1024\n    },\n    \"innerRadius\": {\n      \"type\": \"number\",\n      \"description\": \"Inner radius for star.\",\n      \"example\": 72.0\n    },\n    \"filled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the path has a fill.\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"fillColor\": {\n      \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"stroked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the path has a stroke.\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"strokeColor\": {\n      \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"strokeWidth\": {\n      \"type\": \"number\",\n      \"description\": \"Stroke width in points.\",\n      \"default\": 1,\n      \"example\": 72.0\n    },\n    \"opacity\": {\n      \"type\": \"\
  number\",\n      \"description\": \"Opacity as a percentage (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"default\": 100,\n      \"example\": 72.0\n    },\n    \"layer\": {\n      \"type\": \"string\",\n      \"description\": \"Target layer name.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-path-item-create-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: PathItemCreate
---
