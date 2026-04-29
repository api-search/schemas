---
description: Request body for zip file extraction
layout: schema
name: FileExtractRequest
properties_list:
- description: Path to the zip file in the developer file system
  name: path
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/source-code-api-file-extract-request-schema.json
slug: source-code-api-file-extract-request
source_filename: source-code-api-file-extract-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-file-extract-request-schema.json\",\n  \"title\": \"FileExtractRequest\",\n  \"description\": \"Request body for zip file extraction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the zip file in the developer file system\",\n      \"example\": \"uploads/theme-update.zip\"\n    }\n  },\n  \"required\": [\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-file-extract-request-schema.json
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
title: FileExtractRequest
---
