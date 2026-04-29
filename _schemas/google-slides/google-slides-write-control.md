---
description: Provides control over how write requests are executed. When a write request is made, the requiredRevisionId can be specified to indicate that the write should only succeed if the presentation's current revision matches the specified value.
layout: schema
name: WriteControl
properties_list:
- description: The revision ID of the presentation required for the write request. If specified, the write request is only processed if the current revision ID of the presentation matches this value.
  name: requiredRevisionId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-write-control-schema.json
slug: google-slides-write-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WriteControl\",\n  \"type\": \"object\",\n  \"description\": \"Provides control over how write requests are executed. When a write request is made, the requiredRevisionId can be specified to indicate that the write should only succeed if the presentation's current revision matches the specified value.\\n\",\n  \"properties\": {\n    \"requiredRevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The revision ID of the presentation required for the write request. If specified, the write request is only processed if the current revision ID of the presentation matches this value.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-write-control-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: WriteControl
---
