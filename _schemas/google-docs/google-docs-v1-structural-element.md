---
description: A StructuralElement describes content that provides structure to the document.
layout: schema
name: StructuralElement
properties_list:
- description: The zero-based start index of this structural element.
  name: startIndex
  type: integer
- description: The zero-based end index of this structural element, exclusive.
  name: endIndex
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-structural-element-schema.json
slug: google-docs-v1-structural-element
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StructuralElement\",\n  \"type\": \"object\",\n  \"description\": \"A StructuralElement describes content that provides structure to the document.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based start index of this structural element.\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based end index of this structural element, exclusive.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-structural-element-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: StructuralElement
---
