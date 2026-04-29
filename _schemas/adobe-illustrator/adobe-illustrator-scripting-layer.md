---
description: Layer from Adobe Illustrator API
layout: schema
name: Layer
properties_list:
- description: Unique identifier of the layer.
  name: id
  type: string
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
- description: Whether to dim placed images.
  name: dimPlacedImages
  type: boolean
- description: The layer highlight color.
  name: color
  type: string
- description: Layer opacity as a percentage (0-100).
  name: opacity
  type: number
- description: Blending mode for the layer.
  name: blendingMode
  type: string
- description: Whether the layer is a clipping mask.
  name: isClippingMask
  type: boolean
- description: Whether the layer is sliced.
  name: sliced
  type: boolean
- description: Whether the layer contains selected artwork.
  name: hasSelectedArtwork
  type: boolean
- description: Number of path items in the layer.
  name: pathItemCount
  type: integer
- description: Number of text frames in the layer.
  name: textFrameCount
  type: integer
- description: Number of sublayers.
  name: sublayerCount
  type: integer
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-layer-schema.json
slug: adobe-illustrator-scripting-layer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-layer-schema.json\",\n  \"title\": \"Layer\",\n  \"description\": \"Layer from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the layer.\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the layer.\",\n      \"examples\": [\n        \"Layer 1\"\n      ],\n      \"example\": \"Example Artboard\"\n    },\n    \"visible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is visible.\",\n      \"example\": true\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is locked.\",\n      \"example\": true\n    },\n \
  \   \"printable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is printable.\",\n      \"example\": true\n    },\n    \"preview\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is in preview mode.\",\n      \"example\": true\n    },\n    \"dimPlacedImages\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to dim placed images.\",\n      \"example\": true\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"The layer highlight color.\",\n      \"enum\": [\n        \"Red\",\n        \"Orange\",\n        \"Yellow\",\n        \"Green\",\n        \"Blue\",\n        \"Violet\",\n        \"Gray\",\n        \"LightBlue\",\n        \"LightGreen\",\n        \"LightRed\"\n      ],\n      \"example\": \"Red\"\n    },\n    \"opacity\": {\n      \"type\": \"number\",\n      \"description\": \"Layer opacity as a percentage (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\"\
  : 72.0\n    },\n    \"blendingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Blending mode for the layer.\",\n      \"enum\": [\n        \"Normal\",\n        \"Multiply\",\n        \"Screen\",\n        \"Overlay\",\n        \"Darken\",\n        \"Lighten\",\n        \"ColorDodge\",\n        \"ColorBurn\",\n        \"HardLight\",\n        \"SoftLight\",\n        \"Difference\",\n        \"Exclusion\",\n        \"Hue\",\n        \"Saturation\",\n        \"Color\",\n        \"Luminosity\"\n      ],\n      \"example\": \"Normal\"\n    },\n    \"isClippingMask\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is a clipping mask.\",\n      \"example\": true\n    },\n    \"sliced\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer is sliced.\",\n      \"example\": true\n    },\n    \"hasSelectedArtwork\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the layer contains selected artwork.\",\n      \"\
  example\": true\n    },\n    \"pathItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of path items in the layer.\",\n      \"example\": 1024\n    },\n    \"textFrameCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of text frames in the layer.\",\n      \"example\": 1024\n    },\n    \"sublayerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of sublayers.\",\n      \"example\": 1024\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-layer-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Layer
---
