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
schema_file: json-schema/hubspot-source-code-file-upload-request-schema.json
slug: hubspot-source-code-file-upload-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for file upload operations\",\n  \"properties\": {\n    \"file\": {\n      \"type\": \"string\",\n      \"description\": \"The file content to upload\",\n      \"format\": \"binary\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"file\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FileUploadRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-file-upload-request-schema.json
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
