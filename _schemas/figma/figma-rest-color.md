---
description: An RGBA color value with channels ranging from 0 to 1.
layout: schema
name: Color
properties_list:
- description: Red channel value, between 0 and 1.
  name: r
  type: number
- description: Green channel value, between 0 and 1.
  name: g
  type: number
- description: Blue channel value, between 0 and 1.
  name: b
  type: number
- description: Alpha channel value, between 0 and 1.
  name: a
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-color-schema.json
slug: figma-rest-color
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Color\",\n  \"type\": \"object\",\n  \"description\": \"An RGBA color value with channels ranging from 0 to 1.\",\n  \"properties\": {\n    \"r\": {\n      \"type\": \"number\",\n      \"description\": \"Red channel value, between 0 and 1.\"\n    },\n    \"g\": {\n      \"type\": \"number\",\n      \"description\": \"Green channel value, between 0 and 1.\"\n    },\n    \"b\": {\n      \"type\": \"number\",\n      \"description\": \"Blue channel value, between 0 and 1.\"\n    },\n    \"a\": {\n      \"type\": \"number\",\n      \"description\": \"Alpha channel value, between 0 and 1.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-color-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Color
---
