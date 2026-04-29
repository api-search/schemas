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
source_filename: blender-bpy-operator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blender/main/json-schema/blender-bpy-operator-schema.json\",\n  \"title\": \"Blender bpy Operator\",\n  \"description\": \"Schema representing a Blender Python API operator definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bl_idname\": {\n      \"type\": \"string\",\n      \"description\": \"Operator identifier (e.g., object.transform_apply)\",\n      \"pattern\": \"^[a-z_]+\\\\.[a-z_]+$\"\n    },\n    \"bl_label\": { \"type\": \"string\", \"description\": \"Human-readable operator label\" },\n    \"bl_description\": { \"type\": \"string\", \"description\": \"Tooltip description shown in Blender UI\" },\n    \"bl_options\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"REGISTER\", \"UNDO\", \"BLOCKING\", \"MACRO\", \"GRAB_CURSOR\", \"PRESET\", \"INTERNAL\"]\n      },\n   \
  \   \"description\": \"Operator behavior flags\"\n    },\n    \"poll\": {\n      \"type\": \"string\",\n      \"description\": \"Context poll method description (Python expression or docstring)\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Operator properties exposed via RNA\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"BoolProperty\", \"IntProperty\", \"FloatProperty\", \"StringProperty\", \"EnumProperty\", \"CollectionProperty\"] },\n          \"default\": {},\n          \"description\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"bl_idname\", \"bl_label\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blender/refs/heads/main/json-schema/blender-bpy-operator-schema.json
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
