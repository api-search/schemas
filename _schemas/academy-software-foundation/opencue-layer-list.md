---
description: List of layers
layout: schema
name: LayerList
properties_list:
- description: ''
  name: layers
  type: array
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-layer-list-schema.json
slug: opencue-layer-list
source_filename: opencue-layer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-layer-list-schema.json\",\n  \"title\": \"LayerList\",\n  \"description\": \"List of layers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"layers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Layer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-layer-list-schema.json
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
title: LayerList
---
