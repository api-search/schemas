---
description: A group of detected rich result items of a single type.
layout: schema
name: DetectedItems
properties_list:
- description: The rich result type detected (e.g., Product, Recipe, FAQ, BreadcrumbList, Article).
  name: richResultType
  type: string
- description: The individual detected items of this type.
  name: items
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-detected-items-schema.json
slug: google-search-console-detected-items
source_filename: google-search-console-detected-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DetectedItems\",\n  \"type\": \"object\",\n  \"description\": \"A group of detected rich result items of a single type.\",\n  \"properties\": {\n    \"richResultType\": {\n      \"type\": \"string\",\n      \"description\": \"The rich result type detected (e.g., Product, Recipe, FAQ, BreadcrumbList, Article).\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The individual detected items of this type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-detected-items-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: DetectedItems
---
