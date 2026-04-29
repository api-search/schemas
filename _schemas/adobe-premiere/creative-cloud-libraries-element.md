---
description: A design element within a Creative Cloud Library.
layout: schema
name: Element
properties_list:
- description: Unique identifier of the element.
  name: id
  type: string
- description: Display name of the element.
  name: name
  type: string
- description: Type of the element.
  name: type
  type: string
- description: Timestamp when the element was created.
  name: created_date
  type: string
- description: Timestamp when the element was last modified.
  name: modified_date
  type: string
- description: Renditions and format-specific representations of the element.
  name: representations
  type: array
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-element-schema.json
slug: creative-cloud-libraries-element
source_filename: creative-cloud-libraries-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-schema.json\",\n  \"title\": \"Element\",\n  \"description\": \"A design element within a Creative Cloud Library.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the element.\",\n      \"example\": \"elem-xyz789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the element.\",\n      \"example\": \"Brand Blue Color\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the element.\",\n      \"enum\": [\n        \"color\",\n        \"characterstyle\",\n        \"brushstyle\",\n        \"graphic\",\n        \"pattern\",\n        \"video\"\n      ],\n      \"example\": \"color\"\n    },\n    \"created_date\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the element was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the element was last modified.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"description\": \"Renditions and format-specific representations of the element.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Representation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: Element
---
