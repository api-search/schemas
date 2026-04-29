---
description: Deletes a Footer from the document.
layout: schema
name: DeleteFooterRequest
properties_list:
- description: The ID of the footer to delete.
  name: footerId
  type: string
- description: The tab containing the footer to delete.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-delete-footer-request-schema.json
slug: google-docs-v1-delete-footer-request
source_filename: google-docs-v1-delete-footer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteFooterRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes a Footer from the document.\",\n  \"properties\": {\n    \"footerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the footer to delete.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab containing the footer to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-delete-footer-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DeleteFooterRequest
---
