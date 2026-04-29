---
description: Request body for file upload operations
layout: schema
name: FileUploadRequest
properties_list:
- description: The file content to upload
  name: file
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/source-code-api-file-upload-request-schema.json
slug: source-code-api-file-upload-request
source_filename: source-code-api-file-upload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-file-upload-request-schema.json\",\n  \"title\": \"FileUploadRequest\",\n  \"description\": \"Request body for file upload operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"The file content to upload\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"file\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-file-upload-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: FileUploadRequest
---
