---
description: A USD layer — the fundamental unit of composition in OpenUSD, representing a file or in-memory container for scene description data including prim specs, property specs, and composition arcs.
layout: schema
name: USDLayer
properties_list:
- description: The unique identifier (path or URI) for this layer.
  name: identifier
  type: string
- description: The resolved filesystem path for this layer.
  name: realPath
  type: string
- description: The file format identifier for this layer.
  name: fileFormat
  type: string
- description: The default prim path to use when referencing this layer.
  name: defaultPrim
  type: string
- description: The start time code for the layer's time-sampled data.
  name: startTimeCode
  type: number
- description: The end time code for the layer's time-sampled data.
  name: endTimeCode
  type: number
- description: Frames per second for time code interpretation.
  name: framesPerSecond
  type: number
- description: Time codes per second (usually matches framesPerSecond).
  name: timeCodesPerSecond
  type: number
- description: Scene scale in meters per USD unit.
  name: metersPerUnit
  type: number
- description: The up axis convention for the scene.
  name: upAxis
  type: string
- description: Human-readable documentation for the layer.
  name: documentation
  type: string
- description: Ordered list of sublayer paths composed by this layer.
  name: subLayerPaths
  type: array
provider_name: Alliance for OpenUSD
provider_slug: aousd
schema_file: json-schema/aousd-usd-layer-schema.json
slug: aousd-usd-layer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aousd/refs/heads/main/json-schema/aousd-usd-layer-schema.json\",\n  \"title\": \"USDLayer\",\n  \"description\": \"A USD layer — the fundamental unit of composition in OpenUSD, representing a file or in-memory container for scene description data including prim specs, property specs, and composition arcs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\"type\": \"string\", \"description\": \"The unique identifier (path or URI) for this layer.\", \"example\": \"/assets/characters/hero/hero.usda\"},\n    \"realPath\": {\"type\": \"string\", \"description\": \"The resolved filesystem path for this layer.\", \"example\": \"/studio/assets/characters/hero/hero.usda\"},\n    \"fileFormat\": {\"type\": \"string\", \"description\": \"The file format identifier for this layer.\", \"enum\": [\"usda\", \"usdb\", \"usd\", \"usdz\"], \"\
  example\": \"usda\"},\n    \"defaultPrim\": {\"type\": \"string\", \"description\": \"The default prim path to use when referencing this layer.\", \"example\": \"Hero\"},\n    \"startTimeCode\": {\"type\": \"number\", \"description\": \"The start time code for the layer's time-sampled data.\", \"example\": 1.0},\n    \"endTimeCode\": {\"type\": \"number\", \"description\": \"The end time code for the layer's time-sampled data.\", \"example\": 240.0},\n    \"framesPerSecond\": {\"type\": \"number\", \"description\": \"Frames per second for time code interpretation.\", \"example\": 24.0},\n    \"timeCodesPerSecond\": {\"type\": \"number\", \"description\": \"Time codes per second (usually matches framesPerSecond).\", \"example\": 24.0},\n    \"metersPerUnit\": {\"type\": \"number\", \"description\": \"Scene scale in meters per USD unit.\", \"example\": 0.01},\n    \"upAxis\": {\"type\": \"string\", \"enum\": [\"Y\", \"Z\"], \"description\": \"The up axis convention for the scene.\", \"example\"\
  : \"Y\"},\n    \"documentation\": {\"type\": \"string\", \"description\": \"Human-readable documentation for the layer.\", \"example\": \"Hero character asset for production.\"},\n    \"subLayerPaths\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"Ordered list of sublayer paths composed by this layer.\", \"example\": [\"/assets/characters/hero/hero_rig.usda\", \"/assets/characters/hero/hero_model.usda\"]}\n  },\n  \"required\": [\"identifier\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aousd/refs/heads/main/json-schema/aousd-usd-layer-schema.json
tags:
- 3D
- Interoperability
- Linux Foundation
- Metaverse
- OpenUSD
- Specification
- Standards
- USD
- Visual Effects
title: USDLayer
---
