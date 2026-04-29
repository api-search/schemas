---
description: Location at the end of a body, header, footer, or footnote.
layout: schema
name: EndOfSegmentLocation
properties_list:
- description: The ID of the header, footer, or footnote the location is in. An empty segment ID signifies the document body.
  name: segmentId
  type: string
- description: The tab that the location is in.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-end-of-segment-location-schema.json
slug: google-docs-v1-end-of-segment-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EndOfSegmentLocation\",\n  \"type\": \"object\",\n  \"description\": \"Location at the end of a body, header, footer, or footnote.\",\n  \"properties\": {\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the header, footer, or footnote the location is in. An empty segment ID signifies the document body.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab that the location is in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-end-of-segment-location-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: EndOfSegmentLocation
---
