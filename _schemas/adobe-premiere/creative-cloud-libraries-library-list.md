---
description: Paginated list of Creative Cloud Libraries.
layout: schema
name: LibraryList
properties_list:
- description: Array of library objects.
  name: libraries
  type: array
- description: Total number of libraries available.
  name: total_count
  type: integer
- description: Starting index of the current page.
  name: start
  type: integer
- description: Maximum results per page.
  name: limit
  type: integer
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-library-list-schema.json
slug: creative-cloud-libraries-library-list
source_filename: creative-cloud-libraries-library-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-list-schema.json\",\n  \"title\": \"LibraryList\",\n  \"description\": \"Paginated list of Creative Cloud Libraries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"libraries\": {\n      \"type\": \"array\",\n      \"description\": \"Array of library objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Library\"\n      }\n    },\n    \"total_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of libraries available.\",\n      \"example\": 15\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index of the current page.\",\n      \"example\": 0\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results per page.\",\n      \"example\": 20\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-list-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: LibraryList
---
