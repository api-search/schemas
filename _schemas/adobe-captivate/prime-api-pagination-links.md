---
description: Pagination links following JSON:API conventions
layout: schema
name: PaginationLinks
properties_list:
- description: URL for the current page
  name: self
  type: string
- description: URL for the next page
  name: next
  type: string
- description: URL for the previous page
  name: prev
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-pagination-links-schema.json
slug: prime-api-pagination-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-pagination-links-schema.json\",\n  \"title\": \"PaginationLinks\",\n  \"description\": \"Pagination links following JSON:API conventions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the current page\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the next page\"\n    },\n    \"prev\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the previous page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-pagination-links-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: PaginationLinks
---
