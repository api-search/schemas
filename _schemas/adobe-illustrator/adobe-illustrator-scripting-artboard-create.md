---
description: ArtboardCreate from Adobe Illustrator API
layout: schema
name: ArtboardCreate
properties_list:
- description: Name of the artboard.
  name: name
  type: string
- description: Bounding rectangle [left, top, right, bottom] in points.
  name: artboardRect
  type: array
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-artboard-create-schema.json
slug: adobe-illustrator-scripting-artboard-create
source_filename: adobe-illustrator-scripting-artboard-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-artboard-create-schema.json\",\n  \"title\": \"ArtboardCreate\",\n  \"description\": \"ArtboardCreate from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the artboard.\",\n      \"example\": \"Example Artboard\"\n    },\n    \"artboardRect\": {\n      \"type\": \"array\",\n      \"description\": \"Bounding rectangle [left, top, right, bottom] in points.\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"minItems\": 4,\n      \"maxItems\": 4\n    }\n  },\n  \"required\": [\n    \"artboardRect\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-artboard-create-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: ArtboardCreate
---
