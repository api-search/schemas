---
description: A stock content category
layout: schema
name: Category
properties_list:
- description: Unique category identifier
  name: id
  type: integer
- description: Localized category name
  name: name
  type: string
- description: URL to browse this category on the Adobe Stock website
  name: link
  type: string
- description: Child subcategories (present in category tree responses)
  name: children
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-category-schema.json
slug: adobe-creative-suite-stock-category
source_filename: adobe-creative-suite-stock-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-category-schema.json\",\n  \"title\": \"Category\",\n  \"description\": \"A stock content category\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique category identifier\",\n      \"example\": 1043\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Localized category name\",\n      \"example\": \"Nature\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"URL to browse this category on the Adobe Stock website\",\n      \"example\": \"example_value\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"Child subcategories (present in category tree responses)\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Category\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-category-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: Category
---
