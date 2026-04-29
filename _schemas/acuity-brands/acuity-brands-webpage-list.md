---
description: Paginated list of web pages
layout: schema
name: WebpageList
properties_list:
- description: ''
  name: pages
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: cursor
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-webpage-list-schema.json
slug: acuity-brands-webpage-list
source_filename: acuity-brands-webpage-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-webpage-list-schema.json\",\n  \"title\": \"WebpageList\",\n  \"description\": \"Paginated list of web pages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Webpage\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 10000\n    },\n    \"cursor\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-webpage-list-schema.json
tags: []
title: WebpageList
---
