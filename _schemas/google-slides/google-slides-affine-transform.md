---
description: A 3x3 matrix that represents an affine transformation. The matrix maps a source coordinate (x, y) to a destination coordinate (x', y') according to matrix multiplication.
layout: schema
name: AffineTransform
properties_list:
- description: The X coordinate scaling element.
  name: scaleX
  type: number
- description: The Y coordinate scaling element.
  name: scaleY
  type: number
- description: The X coordinate shearing element.
  name: shearX
  type: number
- description: The Y coordinate shearing element.
  name: shearY
  type: number
- description: The X coordinate translation element.
  name: translateX
  type: number
- description: The Y coordinate translation element.
  name: translateY
  type: number
- description: The units for translate elements.
  name: unit
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-affine-transform-schema.json
slug: google-slides-affine-transform
source_filename: google-slides-affine-transform-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AffineTransform\",\n  \"type\": \"object\",\n  \"description\": \"A 3x3 matrix that represents an affine transformation. The matrix maps a source coordinate (x, y) to a destination coordinate (x', y') according to matrix multiplication.\\n\",\n  \"properties\": {\n    \"scaleX\": {\n      \"type\": \"number\",\n      \"description\": \"The X coordinate scaling element.\"\n    },\n    \"scaleY\": {\n      \"type\": \"number\",\n      \"description\": \"The Y coordinate scaling element.\"\n    },\n    \"shearX\": {\n      \"type\": \"number\",\n      \"description\": \"The X coordinate shearing element.\"\n    },\n    \"shearY\": {\n      \"type\": \"number\",\n      \"description\": \"The Y coordinate shearing element.\"\n    },\n    \"translateX\": {\n      \"type\": \"number\",\n      \"description\": \"The X coordinate translation element.\"\n    },\n    \"translateY\": {\n      \"type\":\
  \ \"number\",\n      \"description\": \"The Y coordinate translation element.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The units for translate elements.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-affine-transform-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: AffineTransform
---
