---
description: DocumentCreate from Adobe Illustrator API
layout: schema
name: DocumentCreate
properties_list:
- description: Name of the new document.
  name: name
  type: string
- description: Color mode of the document.
  name: documentColorSpace
  type: string
- description: Document width in points.
  name: width
  type: number
- description: Document height in points.
  name: height
  type: number
- description: Number of artboards to create.
  name: numArtboards
  type: integer
- description: Layout for multiple artboards.
  name: artboardLayout
  type: string
- description: Raster effects resolution.
  name: rasterResolution
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-document-create-schema.json
slug: adobe-illustrator-scripting-document-create
source_filename: adobe-illustrator-scripting-document-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-document-create-schema.json\",\n  \"title\": \"DocumentCreate\",\n  \"description\": \"DocumentCreate from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the new document.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"documentColorSpace\": {\n      \"type\": \"string\",\n      \"description\": \"Color mode of the document.\",\n      \"enum\": [\n        \"CMYK\",\n        \"RGB\"\n      ],\n      \"default\": \"RGB\",\n      \"example\": \"CMYK\"\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Document width in points.\",\n      \"default\": 612,\n      \"example\": 72.0\n    },\n    \"height\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"Document height in points.\",\n      \"default\": 792,\n      \"example\": 72.0\n    },\n    \"numArtboards\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of artboards to create.\",\n      \"default\": 1,\n      \"example\": 1024\n    },\n    \"artboardLayout\": {\n      \"type\": \"string\",\n      \"description\": \"Layout for multiple artboards.\",\n      \"enum\": [\n        \"GridByRow\",\n        \"GridByCol\",\n        \"Row\",\n        \"Column\",\n        \"RLGridByRow\",\n        \"RLGridByCol\",\n        \"RLRow\"\n      ],\n      \"example\": \"GridByRow\"\n    },\n    \"rasterResolution\": {\n      \"type\": \"string\",\n      \"description\": \"Raster effects resolution.\",\n      \"enum\": [\n        \"ScreenResolution\",\n        \"MediumResolution\",\n        \"HighResolution\"\n      ],\n      \"default\": \"HighResolution\",\n      \"example\": \"ScreenResolution\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-document-create-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: DocumentCreate
---
