---
description: A particular location in the document.
layout: schema
name: Location
properties_list:
- description: The ID of the header, footer, or footnote the location is in. An empty segment ID signifies the document body.
  name: segmentId
  type: string
- description: The zero-based index, in UTF-16 code units. The index is relative to the beginning of the segment specified by segmentId.
  name: index
  type: integer
- description: The tab that the location is in.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-location-schema.json
slug: google-docs-v1-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"description\": \"A particular location in the document.\",\n  \"properties\": {\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the header, footer, or footnote the location is in. An empty segment ID signifies the document body.\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based index, in UTF-16 code units. The index is relative to the beginning of the segment specified by segmentId.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab that the location is in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-location-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Location
---
