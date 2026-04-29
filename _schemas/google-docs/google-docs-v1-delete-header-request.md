---
description: Deletes a Header from the document.
layout: schema
name: DeleteHeaderRequest
properties_list:
- description: The ID of the header to delete.
  name: headerId
  type: string
- description: The tab containing the header to delete.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-delete-header-request-schema.json
slug: google-docs-v1-delete-header-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteHeaderRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes a Header from the document.\",\n  \"properties\": {\n    \"headerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the header to delete.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab containing the header to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-delete-header-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DeleteHeaderRequest
---
