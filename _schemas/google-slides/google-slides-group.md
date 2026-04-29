---
description: A PageElement kind representing a joined collection of PageElements.
layout: schema
name: Group
properties_list:
- description: The collection of elements in the group.
  name: children
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-group-schema.json
slug: google-slides-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing a joined collection of PageElements.\\n\",\n  \"properties\": {\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of elements in the group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-group-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Group
---
