---
description: Request body for creating a library element.
layout: schema
name: ElementInput
properties_list:
- description: Name of the element.
  name: name
  type: string
- description: Type of the element.
  name: type
  type: string
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-element-input-schema.json
slug: creative-cloud-libraries-element-input
source_filename: creative-cloud-libraries-element-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-input-schema.json\",\n  \"title\": \"ElementInput\",\n  \"description\": \"Request body for creating a library element.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the element.\",\n      \"example\": \"Brand Red\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the element.\",\n      \"enum\": [\n        \"color\",\n        \"characterstyle\",\n        \"brushstyle\",\n        \"graphic\",\n        \"pattern\",\n        \"video\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-input-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: ElementInput
---
