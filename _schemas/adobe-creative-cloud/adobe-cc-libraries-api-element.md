---
description: Element from Adobe API
layout: schema
name: Element
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: Element MIME type (e.g., application/vnd.adobe.element.color+dcx).
  name: type
  type: string
- description: ''
  name: created_date
  type: string
- description: ''
  name: modified_date
  type: string
- description: ''
  name: thumbnail
  type: object
- description: Available representations of the element.
  name: representations
  type: array
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-cc-libraries-api-element-schema.json
slug: adobe-cc-libraries-api-element
source_filename: adobe-cc-libraries-api-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-element-schema.json\",\n  \"title\": \"Element\",\n  \"description\": \"Element from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Asset\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Element MIME type (e.g., application/vnd.adobe.element.color+dcx).\",\n      \"example\": \"image\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n   \
  \ },\n    \"thumbnail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"type\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"description\": \"Available representations of the element.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"storage_href\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"content_length\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-element-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: Element
---
