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
source_filename: blender-addon-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blender/main/json-schema/blender-addon-manifest-schema.json\",\n  \"title\": \"Blender Addon Manifest\",\n  \"description\": \"Schema for a Blender addon extension manifest (blender_manifest.toml equivalent in JSON)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schema_version\": { \"type\": \"string\", \"description\": \"Manifest schema version\", \"example\": \"1.0.0\" },\n    \"id\": { \"type\": \"string\", \"description\": \"Unique addon ID (lowercase, underscores)\", \"pattern\": \"^[a-z][a-z0-9_]*$\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Human-readable addon display name\" },\n    \"version\": { \"type\": \"string\", \"description\": \"Addon version (semver)\", \"example\": \"1.2.0\" },\n    \"tagline\": { \"type\": \"string\", \"maxLength\": 64, \"description\": \"Short one-line description\" },\n    \"maintainer\"\
  : { \"type\": \"string\", \"description\": \"Maintainer name and email\" },\n    \"type\": { \"type\": \"string\", \"enum\": [\"add-on\", \"theme\"], \"description\": \"Extension type\" },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Category tags for the Extensions Platform\"\n    },\n    \"blender_version_min\": { \"type\": \"string\", \"description\": \"Minimum supported Blender version\", \"example\": \"4.0.0\" },\n    \"blender_version_max\": { \"type\": \"string\", \"description\": \"Maximum tested Blender version\" },\n    \"license\": { \"type\": \"array\", \"items\": { \"type\": \"string\" }, \"description\": \"SPDX license identifiers\" },\n    \"website\": { \"type\": \"string\", \"format\": \"uri\" }\n  },\n  \"required\": [\"schema_version\", \"id\", \"name\", \"version\", \"type\", \"blender_version_min\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blender/refs/heads/main/json-schema/blender-addon-manifest-schema.json
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
