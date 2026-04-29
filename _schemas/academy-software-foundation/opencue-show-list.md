---
description: List of shows
layout: schema
name: ShowList
properties_list:
- description: ''
  name: shows
  type: array
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-show-list-schema.json
slug: opencue-show-list
source_filename: opencue-show-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-show-list-schema.json\",\n  \"title\": \"ShowList\",\n  \"description\": \"List of shows\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Show\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-show-list-schema.json
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
title: ShowList
---
