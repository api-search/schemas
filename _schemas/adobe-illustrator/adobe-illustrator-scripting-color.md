---
description: Color from Adobe Illustrator API
layout: schema
name: Color
properties_list:
- description: Type of color specification.
  name: colorType
  type: string
- description: Red component (0-255) for RGB colors.
  name: red
  type: number
- description: Green component (0-255) for RGB colors.
  name: green
  type: number
- description: Blue component (0-255) for RGB colors.
  name: blue
  type: number
- description: Cyan component (0-100) for CMYK colors.
  name: cyan
  type: number
- description: Magenta component (0-100) for CMYK colors.
  name: magenta
  type: number
- description: Yellow component (0-100) for CMYK colors.
  name: yellow
  type: number
- description: Black component (0-100) for CMYK colors.
  name: black
  type: number
- description: Gray value (0-100) for grayscale colors.
  name: gray
  type: number
- description: Spot color name for spot colors.
  name: spotName
  type: string
- description: Tint percentage for spot colors.
  name: tint
  type: number
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-color-schema.json
slug: adobe-illustrator-scripting-color
source_filename: adobe-illustrator-scripting-color-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-color-schema.json\",\n  \"title\": \"Color\",\n  \"description\": \"Color from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"colorType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of color specification.\",\n      \"enum\": [\n        \"RGB\",\n        \"CMYK\",\n        \"Gray\",\n        \"Spot\",\n        \"Pattern\",\n        \"Gradient\",\n        \"None\"\n      ],\n      \"example\": \"RGB\"\n    },\n    \"red\": {\n      \"type\": \"number\",\n      \"description\": \"Red component (0-255) for RGB colors.\",\n      \"minimum\": 0,\n      \"maximum\": 255,\n      \"example\": 72.0\n    },\n    \"green\": {\n      \"type\": \"number\",\n      \"description\": \"Green component (0-255) for RGB colors.\",\n      \"minimum\"\
  : 0,\n      \"maximum\": 255,\n      \"example\": 72.0\n    },\n    \"blue\": {\n      \"type\": \"number\",\n      \"description\": \"Blue component (0-255) for RGB colors.\",\n      \"minimum\": 0,\n      \"maximum\": 255,\n      \"example\": 72.0\n    },\n    \"cyan\": {\n      \"type\": \"number\",\n      \"description\": \"Cyan component (0-100) for CMYK colors.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"magenta\": {\n      \"type\": \"number\",\n      \"description\": \"Magenta component (0-100) for CMYK colors.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"yellow\": {\n      \"type\": \"number\",\n      \"description\": \"Yellow component (0-100) for CMYK colors.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"black\": {\n      \"type\": \"number\",\n      \"description\": \"Black component (0-100) for CMYK colors.\",\n      \"minimum\": 0,\n  \
  \    \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"gray\": {\n      \"type\": \"number\",\n      \"description\": \"Gray value (0-100) for grayscale colors.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    },\n    \"spotName\": {\n      \"type\": \"string\",\n      \"description\": \"Spot color name for spot colors.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"tint\": {\n      \"type\": \"number\",\n      \"description\": \"Tint percentage for spot colors.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-color-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Color
---
