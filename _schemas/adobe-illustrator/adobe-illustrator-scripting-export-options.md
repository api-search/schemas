---
description: ExportOptions from Adobe Illustrator API
layout: schema
name: ExportOptions
properties_list:
- description: File path for the exported file.
  name: filePath
  type: string
- description: Export format.
  name: format
  type: string
- description: Range of artboards to export (e.g., "1-3" or "1,3,5"). Empty string exports all artboards.
  name: artboardRange
  type: string
- description: Horizontal scaling factor as a percentage.
  name: horizontalScale
  type: number
- description: Vertical scaling factor as a percentage.
  name: verticalScale
  type: number
- description: Export resolution in PPI.
  name: resolution
  type: number
- description: Whether to use anti-aliasing.
  name: antiAliasing
  type: boolean
- description: Whether to preserve transparency.
  name: transparency
  type: boolean
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-export-options-schema.json
slug: adobe-illustrator-scripting-export-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-export-options-schema.json\",\n  \"title\": \"ExportOptions\",\n  \"description\": \"ExportOptions from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filePath\": {\n      \"type\": \"string\",\n      \"description\": \"File path for the exported file.\",\n      \"example\": \"/path/to/file.ai\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Export format.\",\n      \"enum\": [\n        \"PNG8\",\n        \"PNG24\",\n        \"JPEG\",\n        \"SVG\",\n        \"PDF\",\n        \"TIFF\",\n        \"GIF\",\n        \"AutoCAD\",\n        \"Flash\",\n        \"Photoshop\"\n      ],\n      \"example\": \"PNG8\"\n    },\n    \"artboardRange\": {\n      \"type\": \"string\",\n      \"description\": \"Range of artboards\
  \ to export (e.g., \\\"1-3\\\" or \\\"1,3,5\\\"). Empty string exports all artboards.\",\n      \"default\": \"\",\n      \"example\": \"example_value\"\n    },\n    \"horizontalScale\": {\n      \"type\": \"number\",\n      \"description\": \"Horizontal scaling factor as a percentage.\",\n      \"default\": 100,\n      \"example\": 72.0\n    },\n    \"verticalScale\": {\n      \"type\": \"number\",\n      \"description\": \"Vertical scaling factor as a percentage.\",\n      \"default\": 100,\n      \"example\": 72.0\n    },\n    \"resolution\": {\n      \"type\": \"number\",\n      \"description\": \"Export resolution in PPI.\",\n      \"default\": 72,\n      \"example\": 72.0\n    },\n    \"antiAliasing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use anti-aliasing.\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"transparency\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to preserve transparency.\",\n      \"default\"\
  : true,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"filePath\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-export-options-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: ExportOptions
---
