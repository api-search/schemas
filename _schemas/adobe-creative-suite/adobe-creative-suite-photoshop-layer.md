---
description: Representation of a Photoshop document layer
layout: schema
name: Layer
properties_list:
- description: Unique layer identifier within the document
  name: id
  type: integer
- description: Layer stack index (0 = bottom)
  name: index
  type: integer
- description: Layer name as shown in the Layers panel
  name: name
  type: string
- description: Layer type
  name: type
  type: string
- description: Whether the layer is visible
  name: visible
  type: boolean
- description: Whether the layer is locked
  name: locked
  type: boolean
- description: Layer opacity from 0 to 255
  name: opacity
  type: integer
- description: Blend mode of the layer
  name: blendMode
  type: string
- description: Layer bounding box in pixels
  name: bounds
  type: object
- description: Child layers for group layers
  name: children
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-layer-schema.json
slug: adobe-creative-suite-photoshop-layer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-layer-schema.json\",\n  \"title\": \"Layer\",\n  \"description\": \"Representation of a Photoshop document layer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique layer identifier within the document\",\n      \"example\": 1920\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Layer stack index (0 = bottom)\",\n      \"example\": 1920\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Layer name as shown in the Layers panel\",\n      \"example\": \"Example Asset\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Layer type\",\n      \"enum\": [\n        \"layer\",\n        \"textLayer\",\n        \"adjustmentLayer\"\
  ,\n        \"fillLayer\",\n        \"smartObject\",\n        \"backgroundLayer\",\n        \"groupLayer\"\n      ],\n      \"example\": \"layer\"\n    },\n    \"visible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is visible\",\n      \"example\": true\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is locked\",\n      \"example\": true\n    },\n    \"opacity\": {\n      \"type\": \"integer\",\n      \"description\": \"Layer opacity from 0 to 255\",\n      \"minimum\": 0,\n      \"maximum\": 255,\n      \"example\": 1920\n    },\n    \"blendMode\": {\n      \"type\": \"string\",\n      \"description\": \"Blend mode of the layer\",\n      \"example\": \"normal\"\n    },\n    \"bounds\": {\n      \"type\": \"object\",\n      \"description\": \"Layer bounding box in pixels\",\n      \"properties\": {\n        \"top\": {\n          \"type\": \"integer\"\n        },\n        \"left\": {\n          \"type\"\
  : \"integer\"\n        },\n        \"bottom\": {\n          \"type\": \"integer\"\n        },\n        \"right\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"Child layers for group layers\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Layer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-layer-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: Layer
---
