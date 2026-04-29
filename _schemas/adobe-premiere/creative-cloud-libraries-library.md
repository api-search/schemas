---
description: A Creative Cloud Library containing design elements.
layout: schema
name: Library
properties_list:
- description: Unique identifier of the library.
  name: id
  type: string
- description: Human-readable name of the library.
  name: name
  type: string
- description: ISO 8601 timestamp when the library was created.
  name: created_date
  type: string
- description: ISO 8601 timestamp when the library was last modified.
  name: modified_date
  type: string
- description: Total number of elements in the library.
  name: total_elements
  type: integer
- description: ''
  name: links
  type: object
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-library-schema.json
slug: creative-cloud-libraries-library
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-schema.json\",\n  \"title\": \"Library\",\n  \"description\": \"A Creative Cloud Library containing design elements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the library.\",\n      \"example\": \"lib-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the library.\",\n      \"example\": \"Premiere Pro Brand Assets\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the library was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"ISO 8601 timestamp when the library was last modified.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"total_elements\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of elements in the library.\",\n      \"example\": 42\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/Links\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: Library
---
