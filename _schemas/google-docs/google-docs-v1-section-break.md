---
description: A StructuralElement representing a section break. A section is a range of content that has the same section style.
layout: schema
name: SectionBreak
properties_list:
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-section-break-schema.json
slug: google-docs-v1-section-break
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SectionBreak\",\n  \"type\": \"object\",\n  \"description\": \"A StructuralElement representing a section break. A section is a range of content that has the same section style.\",\n  \"properties\": {\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-section-break-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: SectionBreak
---
