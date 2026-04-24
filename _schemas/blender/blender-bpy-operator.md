---
description: Schema representing a Blender Python API operator definition
layout: schema
name: Blender bpy Operator
properties_list:
- description: Operator identifier (e.g., object.transform_apply)
  name: bl_idname
  type: string
- description: Human-readable operator label
  name: bl_label
  type: string
- description: Tooltip description shown in Blender UI
  name: bl_description
  type: string
- description: Operator behavior flags
  name: bl_options
  type: array
- description: Context poll method description (Python expression or docstring)
  name: poll
  type: string
- description: Operator properties exposed via RNA
  name: properties
  type: array
provider_name: Blender
provider_slug: blender
schema_file: json-schema/blender-bpy-operator-schema.json
slug: blender-bpy-operator
tags:
- 3D
- Animation
- Game Development
- Modeling
- Open Source
- Python
- Rendering
- VFX
title: Blender bpy Operator
---
