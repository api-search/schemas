---
description: A ParagraphElement that represents a run of text that all has the same styling.
layout: schema
name: TextRun
properties_list:
- description: The text of this run. Any non-text elements in the run are replaced with the Unicode character U+E907.
  name: content
  type: string
- description: The suggested insertion IDs.
  name: suggestedInsertionIds
  type: array
- description: The suggested deletion IDs.
  name: suggestedDeletionIds
  type: array
- description: Suggested changes to the text style, keyed by suggestion ID.
  name: suggestedTextStyleChanges
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-text-run-schema.json
slug: google-docs-v1-text-run
source_filename: google-docs-v1-text-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextRun\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement that represents a run of text that all has the same styling.\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The text of this run. Any non-text elements in the run are replaced with the Unicode character U+E907.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\",\n      \"description\": \"The suggested insertion IDs.\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\",\n      \"description\": \"The suggested deletion IDs.\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\",\n      \"description\": \"Suggested changes to the text style, keyed by suggestion ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-text-run-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TextRun
---
