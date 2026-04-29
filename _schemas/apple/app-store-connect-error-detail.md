---
description: ''
layout: schema
name: ErrorDetail
properties_list:
- description: A unique identifier for this error occurrence
  name: id
  type: string
- description: The HTTP status code for this error
  name: status
  type: string
- description: A machine-readable error code
  name: code
  type: string
- description: A short summary of the error
  name: title
  type: string
- description: A detailed explanation of the error
  name: detail
  type: string
- description: ''
  name: source
  type: object
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-error-detail-schema.json
slug: app-store-connect-error-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this error occurrence\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP status code for this error\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"A machine-readable error code\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A short summary of the error\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed explanation of the error\"\n    },\n    \"source\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-error-detail-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: ErrorDetail
---
