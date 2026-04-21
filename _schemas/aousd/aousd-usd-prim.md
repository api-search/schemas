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
