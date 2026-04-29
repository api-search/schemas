---
description: Specifies a range of pages from a PDF document
layout: schema
name: PageRange
properties_list:
- description: Starting page number (1-indexed)
  name: start
  type: integer
- description: Ending page number (1-indexed, inclusive)
  name: end
  type: integer
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-page-range-schema.json
slug: adobe-creative-suite-pdf-services-page-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-page-range-schema.json\",\n  \"title\": \"PageRange\",\n  \"description\": \"Specifies a range of pages from a PDF document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting page number (1-indexed)\",\n      \"example\": 1\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"Ending page number (1-indexed, inclusive)\",\n      \"example\": 5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-page-range-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: PageRange
---
