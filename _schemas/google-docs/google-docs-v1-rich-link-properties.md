---
description: Properties specific to a RichLink.
layout: schema
name: RichLinkProperties
properties_list:
- description: Output only. The title of the RichLink as displayed in the document.
  name: title
  type: string
- description: Output only. The URI of the RichLink.
  name: uri
  type: string
- description: Output only. The MIME type of the RichLink.
  name: mimeType
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-rich-link-properties-schema.json
slug: google-docs-v1-rich-link-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RichLinkProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties specific to a RichLink.\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The title of the RichLink as displayed in the document.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The URI of the RichLink.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The MIME type of the RichLink.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-rich-link-properties-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: RichLinkProperties
---
