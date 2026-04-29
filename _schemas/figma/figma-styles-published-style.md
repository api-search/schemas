---
description: A set of published properties that can be applied to nodes.
layout: schema
name: PublishedStyle
properties_list:
- description: The unique identifier for the style
  name: key
  type: string
- description: The unique identifier of the Figma file that contains the style.
  name: file_key
  type: string
- description: ID of the style node within the figma file
  name: node_id
  type: string
- description: A URL to a thumbnail image of the style.
  name: thumbnail_url
  type: string
- description: The name of the style.
  name: name
  type: string
- description: The description of the style as entered by the publisher.
  name: description
  type: string
- description: The UTC ISO 8601 time when the style was created.
  name: created_at
  type: string
- description: The UTC ISO 8601 time when the style was last updated.
  name: updated_at
  type: string
- description: A user specified order number by which the style can be sorted.
  name: sort_position
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-styles-published-style-schema.json
slug: figma-styles-published-style
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishedStyle\",\n  \"type\": \"object\",\n  \"description\": \"A set of published properties that can be applied to nodes.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the style\"\n    },\n    \"file_key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Figma file that contains the style.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the style node within the figma file\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the style.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the style.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the style as entered by\
  \ the publisher.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the style was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the style was last updated.\"\n    },\n    \"sort_position\": {\n      \"type\": \"string\",\n      \"description\": \"A user specified order number by which the style can be sorted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-styles-published-style-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PublishedStyle
---
