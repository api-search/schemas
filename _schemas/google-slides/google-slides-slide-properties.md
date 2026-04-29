---
description: The properties of a Page that are only relevant for pages with pageType SLIDE.
layout: schema
name: SlideProperties
properties_list:
- description: The object ID of the layout that this slide is based on.
  name: layoutObjectId
  type: string
- description: The object ID of the master that this slide is based on.
  name: masterObjectId
  type: string
- description: Whether the slide is skipped in the presentation mode.
  name: isSkipped
  type: boolean
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-slide-properties-schema.json
slug: google-slides-slide-properties
source_filename: google-slides-slide-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SlideProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Page that are only relevant for pages with pageType SLIDE.\\n\",\n  \"properties\": {\n    \"layoutObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the layout that this slide is based on.\\n\"\n    },\n    \"masterObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the master that this slide is based on.\\n\"\n    },\n    \"isSkipped\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the slide is skipped in the presentation mode.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-slide-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: SlideProperties
---
