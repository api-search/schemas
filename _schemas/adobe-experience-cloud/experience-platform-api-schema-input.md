---
description: SchemaInput schema
layout: schema
name: SchemaInput
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: allOf
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-schema-input-schema.json
slug: experience-platform-api-schema-input
source_filename: experience-platform-api-schema-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-schema-input-schema.json\",\n  \"title\": \"SchemaInput\",\n  \"description\": \"SchemaInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"type\",\n    \"allOf\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"allOf\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"$ref\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-schema-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: SchemaInput
---
