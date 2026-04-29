---
description: Request body for creating a new document. Only the title is used.
layout: schema
name: CreateDocumentRequest
properties_list:
- description: The title of the document to create.
  name: title
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-create-document-request-schema.json
slug: google-docs-v1-create-document-request
source_filename: google-docs-v1-create-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDocumentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new document. Only the title is used.\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the document to create.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-create-document-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: CreateDocumentRequest
---
