---
description: A USD prim — a named container in the scene hierarchy that can have typed schemas, properties, metadata, and composition arcs applied to it.
layout: schema
name: USDPrim
properties_list:
- description: The absolute scene path to this prim.
  name: path
  type: string
- description: The name component of the prim path.
  name: name
  type: string
- description: The typed schema name applied to this prim.
  name: typeName
  type: string
- description: How this prim is introduced into the scene.
  name: specifier
  type: string
- description: Whether this prim is active (inactive prims are excluded from rendering).
  name: active
  type: boolean
- description: Whether this prim is hidden in interactive contexts.
  name: hidden
  type: boolean
- description: The model hierarchy kind of this prim.
  name: kind
  type: string
- description: Documentation string for this prim.
  name: documentation
  type: string
- description: The imaging purpose for this prim.
  name: purpose
  type: string
- description: Whether this prim should be treated as an instance master for instancing.
  name: instanceable
  type: boolean
provider_name: Alliance for OpenUSD
provider_slug: aousd
schema_file: json-schema/aousd-usd-prim-schema.json
slug: aousd-usd-prim
source_filename: aousd-usd-prim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aousd/refs/heads/main/json-schema/aousd-usd-prim-schema.json\",\n  \"title\": \"USDPrim\",\n  \"description\": \"A USD prim — a named container in the scene hierarchy that can have typed schemas, properties, metadata, and composition arcs applied to it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\"type\": \"string\", \"description\": \"The absolute scene path to this prim.\", \"example\": \"/World/Characters/Hero\"},\n    \"name\": {\"type\": \"string\", \"description\": \"The name component of the prim path.\", \"example\": \"Hero\"},\n    \"typeName\": {\"type\": \"string\", \"description\": \"The typed schema name applied to this prim.\", \"example\": \"Xform\"},\n    \"specifier\": {\"type\": \"string\", \"enum\": [\"def\", \"over\", \"class\"], \"description\": \"How this prim is introduced into the scene.\", \"example\"\
  : \"def\"},\n    \"active\": {\"type\": \"boolean\", \"description\": \"Whether this prim is active (inactive prims are excluded from rendering).\", \"example\": true},\n    \"hidden\": {\"type\": \"boolean\", \"description\": \"Whether this prim is hidden in interactive contexts.\", \"example\": false},\n    \"kind\": {\"type\": \"string\", \"enum\": [\"\", \"model\", \"group\", \"assembly\", \"component\", \"subcomponent\"], \"description\": \"The model hierarchy kind of this prim.\", \"example\": \"component\"},\n    \"documentation\": {\"type\": \"string\", \"description\": \"Documentation string for this prim.\", \"example\": \"The hero character asset prim.\"},\n    \"purpose\": {\"type\": \"string\", \"enum\": [\"default\", \"render\", \"proxy\", \"guide\"], \"description\": \"The imaging purpose for this prim.\", \"example\": \"default\"},\n    \"instanceable\": {\"type\": \"boolean\", \"description\": \"Whether this prim should be treated as an instance master for instancing.\"\
  , \"example\": false}\n  },\n  \"required\": [\"path\", \"name\", \"specifier\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aousd/refs/heads/main/json-schema/aousd-usd-prim-schema.json
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
title: USDPrim
---
