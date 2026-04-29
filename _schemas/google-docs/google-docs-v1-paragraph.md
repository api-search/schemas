---
description: A StructuralElement representing a paragraph. A paragraph is a range of content that is terminated with a newline character.
layout: schema
name: Paragraph
properties_list:
- description: The content of the paragraph, broken into its component parts.
  name: elements
  type: array
- description: Suggested changes to the paragraph style, keyed by suggestion ID.
  name: suggestedParagraphStyleChanges
  type: object
- description: Suggested changes to the bullet, keyed by suggestion ID.
  name: suggestedBulletChanges
  type: object
- description: The IDs of the positioned objects tethered to this paragraph.
  name: positionedObjectIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-paragraph-schema.json
slug: google-docs-v1-paragraph
source_filename: google-docs-v1-paragraph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paragraph\",\n  \"type\": \"object\",\n  \"description\": \"A StructuralElement representing a paragraph. A paragraph is a range of content that is terminated with a newline character.\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"description\": \"The content of the paragraph, broken into its component parts.\"\n    },\n    \"suggestedParagraphStyleChanges\": {\n      \"type\": \"object\",\n      \"description\": \"Suggested changes to the paragraph style, keyed by suggestion ID.\"\n    },\n    \"suggestedBulletChanges\": {\n      \"type\": \"object\",\n      \"description\": \"Suggested changes to the bullet, keyed by suggestion ID.\"\n    },\n    \"positionedObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the positioned objects tethered to this paragraph.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-paragraph-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Paragraph
---
