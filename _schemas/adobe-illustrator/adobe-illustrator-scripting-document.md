---
description: Document from Adobe Illustrator API
layout: schema
name: Document
properties_list:
- description: Unique identifier of the document.
  name: id
  type: string
- description: Name of the document.
  name: name
  type: string
- description: Full file path of the document.
  name: fullName
  type: string
- description: Whether the document has been saved.
  name: saved
  type: boolean
- description: The document color mode.
  name: documentColorSpace
  type: string
- description: Document width in points.
  name: width
  type: number
- description: Document height in points.
  name: height
  type: number
- description: Ruler units used in the document.
  name: rulerUnits
  type: string
- description: The ruler origin point [x, y].
  name: rulerOrigin
  type: array
- description: Number of layers in the document.
  name: layerCount
  type: integer
- description: Number of artboards in the document.
  name: artboardCount
  type: integer
- description: Name of the currently active layer.
  name: activeLayer
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-document-schema.json
slug: adobe-illustrator-scripting-document
source_filename: adobe-illustrator-scripting-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-document-schema.json\",\n  \"title\": \"Document\",\n  \"description\": \"Document from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the document.\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the document.\",\n      \"examples\": [\n        \"Untitled-1\"\n      ],\n      \"example\": \"Example Artboard\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full file path of the document.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"saved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the document has been saved.\"\
  ,\n      \"example\": true\n    },\n    \"documentColorSpace\": {\n      \"type\": \"string\",\n      \"description\": \"The document color mode.\",\n      \"enum\": [\n        \"CMYK\",\n        \"RGB\"\n      ],\n      \"example\": \"CMYK\"\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Document width in points.\",\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Document height in points.\",\n      \"example\": 72.0\n    },\n    \"rulerUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Ruler units used in the document.\",\n      \"enum\": [\n        \"Points\",\n        \"Picas\",\n        \"Inches\",\n        \"Millimeters\",\n        \"Centimeters\",\n        \"Pixels\"\n      ],\n      \"example\": \"Points\"\n    },\n    \"rulerOrigin\": {\n      \"type\": \"array\",\n      \"description\": \"The ruler origin point [x, y].\",\n      \"items\": {\n        \"type\": \"number\"\
  \n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"layerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of layers in the document.\",\n      \"example\": 1024\n    },\n    \"artboardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of artboards in the document.\",\n      \"example\": 1024\n    },\n    \"activeLayer\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the currently active layer.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-document-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Document
---
