---
description: LayerCreate from Adobe Illustrator API
layout: schema
name: LayerCreate
properties_list:
- description: Name of the layer.
  name: name
  type: string
- description: Whether the layer is visible.
  name: visible
  type: boolean
- description: Whether the layer is locked.
  name: locked
  type: boolean
- description: Whether the layer is printable.
  name: printable
  type: boolean
- description: Whether the layer is in preview mode.
  name: preview
  type: boolean
- description: Layer opacity as a percentage (0-100).
  name: opacity
  type: number
- description: Blending mode for the layer.
  name: blendingMode
  type: string
- description: Layer highlight color.
  name: color
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-layer-create-schema.json
slug: adobe-illustrator-scripting-layer-create
source_filename: adobe-illustrator-scripting-layer-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-layer-create-schema.json\",\n  \"title\": \"LayerCreate\",\n  \"description\": \"LayerCreate from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the layer.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"visible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is visible.\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is locked.\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"printable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is printable.\",\n      \"default\": true,\n\
  \      \"example\": true\n    },\n    \"preview\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is in preview mode.\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"opacity\": {\n      \"type\": \"number\",\n      \"description\": \"Layer opacity as a percentage (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"default\": 100,\n      \"example\": 72.0\n    },\n    \"blendingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Blending mode for the layer.\",\n      \"enum\": [\n        \"Normal\",\n        \"Multiply\",\n        \"Screen\",\n        \"Overlay\"\n      ],\n      \"default\": \"Normal\",\n      \"example\": \"Normal\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Layer highlight color.\",\n      \"enum\": [\n        \"Red\",\n        \"Orange\",\n        \"Yellow\",\n        \"Green\",\n        \"Blue\",\n        \"Violet\"\n      ],\n      \"example\": \"\
  Red\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-layer-create-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: LayerCreate
---
