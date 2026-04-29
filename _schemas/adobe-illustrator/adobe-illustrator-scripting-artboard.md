---
description: Artboard from Adobe Illustrator API
layout: schema
name: Artboard
properties_list:
- description: Zero-based index of the artboard.
  name: index
  type: integer
- description: Name of the artboard.
  name: name
  type: string
- description: Bounding rectangle [left, top, right, bottom] in points.
  name: artboardRect
  type: array
- description: Ruler origin point [x, y].
  name: rulerOrigin
  type: array
- description: Ruler pixel aspect ratio.
  name: rulerPAR
  type: number
- description: Whether to show the center mark.
  name: showCenter
  type: boolean
- description: Whether to show cross hairs.
  name: showCrossHairs
  type: boolean
- description: Whether to show safe areas.
  name: showSafeAreas
  type: boolean
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-artboard-schema.json
slug: adobe-illustrator-scripting-artboard
source_filename: adobe-illustrator-scripting-artboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-artboard-schema.json\",\n  \"title\": \"Artboard\",\n  \"description\": \"Artboard from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-based index of the artboard.\",\n      \"example\": 1024\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the artboard.\",\n      \"examples\": [\n        \"Artboard 1\"\n      ],\n      \"example\": \"Example Artboard\"\n    },\n    \"artboardRect\": {\n      \"type\": \"array\",\n      \"description\": \"Bounding rectangle [left, top, right, bottom] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 4,\n      \"maxItems\": 4\n    },\n    \"rulerOrigin\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"Ruler origin point [x, y].\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"rulerPAR\": {\n      \"type\": \"number\",\n      \"description\": \"Ruler pixel aspect ratio.\",\n      \"example\": 72.0\n    },\n    \"showCenter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to show the center mark.\",\n      \"example\": true\n    },\n    \"showCrossHairs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to show cross hairs.\",\n      \"example\": true\n    },\n    \"showSafeAreas\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to show safe areas.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-artboard-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Artboard
---
