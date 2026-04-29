---
description: Paginated list of library elements.
layout: schema
name: ElementList
properties_list:
- description: Array of element objects.
  name: elements
  type: array
- description: Total number of elements in the library.
  name: total_count
  type: integer
- description: Starting index of current page.
  name: start
  type: integer
- description: Maximum results per page.
  name: limit
  type: integer
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-element-list-schema.json
slug: creative-cloud-libraries-element-list
source_filename: creative-cloud-libraries-element-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-list-schema.json\",\n  \"title\": \"ElementList\",\n  \"description\": \"Paginated list of library elements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"description\": \"Array of element objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Element\"\n      }\n    },\n    \"total_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of elements in the library.\",\n      \"example\": 8\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index of current page.\",\n      \"example\": 0\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results per page.\",\n      \"example\": 20\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-element-list-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: ElementList
---
