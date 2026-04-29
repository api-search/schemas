---
description: The properties of a Page that are only relevant for pages with pageType LAYOUT.
layout: schema
name: LayoutProperties
properties_list:
- description: The object ID of the master that this layout is based on.
  name: masterObjectId
  type: string
- description: The name of the layout.
  name: name
  type: string
- description: The human-readable name of the layout.
  name: displayName
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-layout-properties-schema.json
slug: google-slides-layout-properties
source_filename: google-slides-layout-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LayoutProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Page that are only relevant for pages with pageType LAYOUT.\\n\",\n  \"properties\": {\n    \"masterObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the master that this layout is based on.\\n\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the layout.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the layout.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-layout-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: LayoutProperties
---
