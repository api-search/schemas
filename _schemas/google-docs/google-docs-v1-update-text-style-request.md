---
description: Updates the styling of text in the document.
layout: schema
name: UpdateTextStyleRequest
properties_list:
- description: The fields that should be updated. At least one field must be specified. The root textStyle is implied and should not be specified. For example, to update the bold field, set fields to "bold".
  name: fields
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-update-text-style-request-schema.json
slug: google-docs-v1-update-text-style-request
source_filename: google-docs-v1-update-text-style-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTextStyleRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the styling of text in the document.\",\n  \"properties\": {\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated. At least one field must be specified. The root textStyle is implied and should not be specified. For example, to update the bold field, set fields to \\\"bold\\\".\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-update-text-style-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: UpdateTextStyleRequest
---
