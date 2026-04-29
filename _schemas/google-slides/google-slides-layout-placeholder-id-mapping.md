---
description: The mapping between a placeholder on a layout and an object ID for the placeholder on a created slide.
layout: schema
name: LayoutPlaceholderIdMapping
properties_list:
- description: The object ID of the placeholder on a layout that will be applied to a slide.
  name: layoutPlaceholderObjectId
  type: string
- description: A user-supplied object ID for the placeholder identified above that is to be created on the corresponding slide.
  name: objectId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-layout-placeholder-id-mapping-schema.json
slug: google-slides-layout-placeholder-id-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LayoutPlaceholderIdMapping\",\n  \"type\": \"object\",\n  \"description\": \"The mapping between a placeholder on a layout and an object ID for the placeholder on a created slide.\\n\",\n  \"properties\": {\n    \"layoutPlaceholderObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the placeholder on a layout that will be applied to a slide.\\n\"\n    },\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID for the placeholder identified above that is to be created on the corresponding slide.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-layout-placeholder-id-mapping-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: LayoutPlaceholderIdMapping
---
