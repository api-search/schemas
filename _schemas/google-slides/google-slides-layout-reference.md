---
description: Slide layout reference.
layout: schema
name: LayoutReference
properties_list:
- description: Predefined layout.
  name: predefinedLayout
  type: string
- description: Layout ID referring to an existing layout in the presentation.
  name: layoutId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-layout-reference-schema.json
slug: google-slides-layout-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LayoutReference\",\n  \"type\": \"object\",\n  \"description\": \"Slide layout reference.\",\n  \"properties\": {\n    \"predefinedLayout\": {\n      \"type\": \"string\",\n      \"description\": \"Predefined layout.\"\n    },\n    \"layoutId\": {\n      \"type\": \"string\",\n      \"description\": \"Layout ID referring to an existing layout in the presentation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-layout-reference-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: LayoutReference
---
