---
description: The properties of a Shape. If the shape is a placeholder shape, then these properties may be inherited from its parent placeholder shape.
layout: schema
name: ShapeProperties
properties_list:
- description: The alignment of the content in the shape.
  name: contentAlignment
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-shape-properties-schema.json
slug: google-slides-shape-properties
source_filename: google-slides-shape-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapeProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Shape. If the shape is a placeholder shape, then these properties may be inherited from its parent placeholder shape.\\n\",\n  \"properties\": {\n    \"contentAlignment\": {\n      \"type\": \"string\",\n      \"description\": \"The alignment of the content in the shape.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-shape-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ShapeProperties
---
