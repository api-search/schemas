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
source_filename: arlula-archive-scene-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/archive-scene.json\",\n  \"title\": \"ArchiveScene\",\n  \"description\": \"A satellite imagery scene available in the archive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ordering ID for the scene.\",\n      \"examples\": [\n        \"scene-a1b2c3d4\"\n      ]\n    },\n    \"supplier\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier identifier.\",\n      \"examples\": [\n        \"supplier-001\"\n      ]\n    },\n    \"captureDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the imagery was captured.\",\n      \"examples\": [\n        \"2025-02-15\"\n      ]\n    },\n    \"gsd\": {\n      \"type\": \"number\",\n      \"description\": \"Ground sample distance in meters.\",\n      \"examples\": [\n        1.5\n      ]\n    },\n    \"cloudCover\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Cloud cover percentage at time of capture.\",\n      \"examples\": [\n        12\n      ]\n    },\n    \"offNadir\": {\n      \"type\": \"number\",\n      \"description\": \"Off-nadir angle at time of capture.\",\n      \"examples\": [\n        15.2\n      ]\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Price for ordering this scene.\",\n      \"examples\": [\n        150.0\n      ]\n    },\n    \"bundles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/bundle.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-archive-scene-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveScene
---
