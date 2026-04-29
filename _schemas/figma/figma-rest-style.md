---
description: A published style that can be applied to nodes in Figma.
layout: schema
name: Style
properties_list:
- description: The globally unique key of the style.
  name: key
  type: string
- description: Name of the style.
  name: name
  type: string
- description: Description of the style.
  name: description
  type: string
- description: Whether this style is a remote style from an external library.
  name: remote
  type: boolean
- description: The type of style.
  name: style_type
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-style-schema.json
slug: figma-rest-style
source_filename: figma-rest-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Style\",\n  \"type\": \"object\",\n  \"description\": \"A published style that can be applied to nodes in Figma.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique key of the style.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the style.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the style.\"\n    },\n    \"remote\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this style is a remote style from an external library.\"\n    },\n    \"style_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of style.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-style-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Style
---
