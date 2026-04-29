---
description: A single detected rich result item.
layout: schema
name: Item
properties_list:
- description: The name or identifier of the rich result item.
  name: name
  type: string
- description: Issues found with this rich result item.
  name: issues
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-item-schema.json
slug: google-search-console-item
source_filename: google-search-console-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Item\",\n  \"type\": \"object\",\n  \"description\": \"A single detected rich result item.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or identifier of the rich result item.\"\n    },\n    \"issues\": {\n      \"type\": \"array\",\n      \"description\": \"Issues found with this rich result item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-item-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: Item
---
