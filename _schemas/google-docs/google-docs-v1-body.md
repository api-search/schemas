---
description: The document body. The body typically contains the full content of the document.
layout: schema
name: Body
properties_list:
- description: The contents of the body. Elements in the body are ordered by their start index.
  name: content
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-body-schema.json
slug: google-docs-v1-body
source_filename: google-docs-v1-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Body\",\n  \"type\": \"object\",\n  \"description\": \"The document body. The body typically contains the full content of the document.\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The contents of the body. Elements in the body are ordered by their start index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-body-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Body
---
