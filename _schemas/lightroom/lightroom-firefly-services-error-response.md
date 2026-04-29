---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error type URI
  name: type
  type: string
- description: Short error description
  name: title
  type: string
- description: Error code
  name: code
  type: integer
- description: Detailed error message
  name: detail
  type: string
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-error-response-schema.json
slug: lightroom-firefly-services-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Error type URI\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short error description\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-error-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: ErrorResponse
---
