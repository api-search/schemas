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
