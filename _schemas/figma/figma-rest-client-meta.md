---
description: Position metadata for a pinned comment. Describes where the comment marker is located on the canvas.
layout: schema
name: ClientMeta
properties_list:
- description: X coordinate of the comment pin.
  name: x
  type: number
- description: Y coordinate of the comment pin.
  name: y
  type: number
- description: The node ID the comment is pinned to.
  name: node_id
  type: string
- description: Offset from the node origin.
  name: node_offset
  type: object
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-client-meta-schema.json
slug: figma-rest-client-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientMeta\",\n  \"type\": \"object\",\n  \"description\": \"Position metadata for a pinned comment. Describes where the comment marker is located on the canvas.\",\n  \"properties\": {\n    \"x\": {\n      \"type\": \"number\",\n      \"description\": \"X coordinate of the comment pin.\"\n    },\n    \"y\": {\n      \"type\": \"number\",\n      \"description\": \"Y coordinate of the comment pin.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node ID the comment is pinned to.\"\n    },\n    \"node_offset\": {\n      \"type\": \"object\",\n      \"description\": \"Offset from the node origin.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-client-meta-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ClientMeta
---
