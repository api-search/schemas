---
description: Replaces the content of the specified NamedRange.
layout: schema
name: ReplaceNamedRangeContentRequest
properties_list:
- description: The ID of the named range whose content will be replaced.
  name: namedRangeId
  type: string
- description: The name of the named ranges whose content will be replaced.
  name: namedRangeName
  type: string
- description: Replaces the content of the specified named range with the given text.
  name: text
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-replace-named-range-content-request-schema.json
slug: google-docs-v1-replace-named-range-content-request
source_filename: google-docs-v1-replace-named-range-content-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceNamedRangeContentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces the content of the specified NamedRange.\",\n  \"properties\": {\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the named range whose content will be replaced.\"\n    },\n    \"namedRangeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the named ranges whose content will be replaced.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Replaces the content of the specified named range with the given text.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-replace-named-range-content-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ReplaceNamedRangeContentRequest
---
