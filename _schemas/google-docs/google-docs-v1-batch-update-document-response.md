---
description: Response message for BatchUpdateDocument.
layout: schema
name: BatchUpdateDocumentResponse
properties_list:
- description: The ID of the document to which the updates were applied.
  name: documentId
  type: string
- description: The reply of the updates. This maps 1:1 with the updates, although replies to some requests may be empty.
  name: replies
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-batch-update-document-response-schema.json
slug: google-docs-v1-batch-update-document-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateDocumentResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for BatchUpdateDocument.\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the document to which the updates were applied.\"\n    },\n    \"replies\": {\n      \"type\": \"array\",\n      \"description\": \"The reply of the updates. This maps 1:1 with the updates, although replies to some requests may be empty.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-batch-update-document-response-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: BatchUpdateDocumentResponse
---
