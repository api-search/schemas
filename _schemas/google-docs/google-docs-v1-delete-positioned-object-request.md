---
description: Deletes a PositionedObject from the document.
layout: schema
name: DeletePositionedObjectRequest
properties_list:
- description: The ID of the positioned object to delete.
  name: objectId
  type: string
- description: The tab that the positioned object is in.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-delete-positioned-object-request-schema.json
slug: google-docs-v1-delete-positioned-object-request
source_filename: google-docs-v1-delete-positioned-object-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletePositionedObjectRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes a PositionedObject from the document.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the positioned object to delete.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab that the positioned object is in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-delete-positioned-object-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DeletePositionedObjectRequest
---
