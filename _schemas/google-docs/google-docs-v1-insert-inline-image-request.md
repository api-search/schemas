---
description: Inserts an InlineObject containing an image at the given location.
layout: schema
name: InsertInlineImageRequest
properties_list:
- description: The image URI. The image is fetched once at insertion time and a copy is stored for display inside the document.
  name: uri
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-insert-inline-image-request-schema.json
slug: google-docs-v1-insert-inline-image-request
source_filename: google-docs-v1-insert-inline-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertInlineImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts an InlineObject containing an image at the given location.\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The image URI. The image is fetched once at insertion time and a copy is stored for display inside the document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-insert-inline-image-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InsertInlineImageRequest
---
