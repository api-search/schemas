---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: detail
  type: string
- description: ''
  name: report
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/data-collection-error-response-schema.json
slug: data-collection-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"detail\": {\n      \"type\": \"string\"\n    },\n    \"report\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/data-collection-error-response-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: ErrorResponse
---
