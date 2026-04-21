---
description: A satellite imagery scene available in the archive.
layout: schema
name: ArchiveScene
properties_list:
- description: Unique ordering ID for the scene.
  name: id
  type: string
- description: Supplier identifier.
  name: supplier
  type: string
- description: Date the imagery was captured.
  name: captureDate
  type: string
- description: Ground sample distance in meters.
  name: gsd
  type: number
- description: Cloud cover percentage at time of capture.
  name: cloudCover
  type: integer
- description: Off-nadir angle at time of capture.
  name: offNadir
  type: number
- description: Price for ordering this scene.
  name: price
  type: number
- description: ''
  name: bundles
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-archive-scene-schema.json
slug: arlula-archive-scene
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveScene
---
