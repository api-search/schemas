---
description: Duplicates a slide or page element. When duplicating a slide, the duplicate slide will be created immediately following the specified slide.
layout: schema
name: DuplicateObjectRequest
properties_list:
- description: The ID of the object to duplicate.
  name: objectId
  type: string
- description: The object being duplicated may contain other objects. This defines how the IDs of duplicated objects are generated.
  name: objectIds
  type: object
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-duplicate-object-request-schema.json
slug: google-slides-duplicate-object-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DuplicateObjectRequest\",\n  \"type\": \"object\",\n  \"description\": \"Duplicates a slide or page element. When duplicating a slide, the duplicate slide will be created immediately following the specified slide.\\n\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the object to duplicate.\"\n    },\n    \"objectIds\": {\n      \"type\": \"object\",\n      \"description\": \"The object being duplicated may contain other objects. This defines how the IDs of duplicated objects are generated.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-duplicate-object-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: DuplicateObjectRequest
---
