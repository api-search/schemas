---
description: A canvas (page) in the Figma document.
layout: schema
name: CanvasNode
properties_list:
- description: A string uniquely identifying this node within the document.
  name: id
  type: string
- description: The name given to the page by the user.
  name: name
  type: string
- description: The type of the node.
  name: type
  type: string
- description: An array of top-level layers on the canvas.
  name: children
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-canvas-node-schema.json
slug: figma-rest-canvas-node
source_filename: figma-rest-canvas-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CanvasNode\",\n  \"type\": \"object\",\n  \"description\": \"A canvas (page) in the Figma document.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A string uniquely identifying this node within the document.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name given to the page by the user.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the node.\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"An array of top-level layers on the canvas.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-canvas-node-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: CanvasNode
---
