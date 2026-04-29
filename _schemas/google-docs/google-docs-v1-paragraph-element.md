---
description: A ParagraphElement describes content within a paragraph.
layout: schema
name: ParagraphElement
properties_list:
- description: The zero-based start index of this paragraph element.
  name: startIndex
  type: integer
- description: The zero-based end index of this paragraph element, exclusive.
  name: endIndex
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-paragraph-element-schema.json
slug: google-docs-v1-paragraph-element
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParagraphElement\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement describes content within a paragraph.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based start index of this paragraph element.\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based end index of this paragraph element, exclusive.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-paragraph-element-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ParagraphElement
---
