---
description: Inserts text at the given location.
layout: schema
name: InsertTextRequest
properties_list:
- description: The text to be inserted. Inserting a newline character will implicitly create a new Paragraph at that index.
  name: text
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-insert-text-request-schema.json
slug: google-docs-v1-insert-text-request
source_filename: google-docs-v1-insert-text-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTextRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts text at the given location.\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text to be inserted. Inserting a newline character will implicitly create a new Paragraph at that index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-insert-text-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InsertTextRequest
---
