---
description: A document footer.
layout: schema
name: Footer
properties_list:
- description: Output only. The ID of the footer.
  name: footerId
  type: string
- description: The contents of the footer.
  name: content
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-footer-schema.json
slug: google-docs-v1-footer
source_filename: google-docs-v1-footer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Footer\",\n  \"type\": \"object\",\n  \"description\": \"A document footer.\",\n  \"properties\": {\n    \"footerId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the footer.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The contents of the footer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-footer-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Footer
---
