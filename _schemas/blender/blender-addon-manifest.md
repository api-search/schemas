---
description: Schema for a Blender addon extension manifest (blender_manifest.toml equivalent in JSON)
layout: schema
name: Blender Addon Manifest
properties_list:
- description: Manifest schema version
  name: schema_version
  type: string
- description: Unique addon ID (lowercase, underscores)
  name: id
  type: string
- description: Human-readable addon display name
  name: name
  type: string
- description: Addon version (semver)
  name: version
  type: string
- description: Short one-line description
  name: tagline
  type: string
- description: Maintainer name and email
  name: maintainer
  type: string
- description: Extension type
  name: type
  type: string
- description: Category tags for the Extensions Platform
  name: tags
  type: array
- description: Minimum supported Blender version
  name: blender_version_min
  type: string
- description: Maximum tested Blender version
  name: blender_version_max
  type: string
- description: SPDX license identifiers
  name: license
  type: array
- description: ''
  name: website
  type: string
provider_name: Blender
provider_slug: blender
schema_file: json-schema/blender-addon-manifest-schema.json
slug: blender-addon-manifest
tags:
- 3D
- Animation
- Game Development
- Modeling
- Open Source
- Python
- Rendering
- VFX
title: Blender Addon Manifest
---
