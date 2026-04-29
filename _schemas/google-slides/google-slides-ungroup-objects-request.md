---
description: Ungroups objects, such as groups.
layout: schema
name: UngroupObjectsRequest
properties_list:
- description: The object IDs of the objects to ungroup. Only groups that are not inside other groups can be ungrouped.
  name: objectIds
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-ungroup-objects-request-schema.json
slug: google-slides-ungroup-objects-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UngroupObjectsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Ungroups objects, such as groups.\",\n  \"properties\": {\n    \"objectIds\": {\n      \"type\": \"array\",\n      \"description\": \"The object IDs of the objects to ungroup. Only groups that are not inside other groups can be ungrouped.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-ungroup-objects-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UngroupObjectsRequest
---
