---
description: ElementCreation from Adobe API
layout: schema
name: ElementCreation
properties_list:
- description: Display name for the element.
  name: name
  type: string
- description: Element MIME type.
  name: type
  type: string
- description: Application-specific metadata.
  name: client_data
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-cc-libraries-api-element-creation-schema.json
slug: adobe-cc-libraries-api-element-creation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-element-creation-schema.json\",\n  \"title\": \"ElementCreation\",\n  \"description\": \"ElementCreation from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the element.\",\n      \"example\": \"Example Asset\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Element MIME type.\",\n      \"example\": \"image\"\n    },\n    \"client_data\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-element-creation-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: ElementCreation
---
