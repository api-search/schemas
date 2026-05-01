---
description: A category that organizes articles within a Document360 knowledge base project version.
layout: schema
name: Document360 Category
properties_list:
- description: Unique identifier for the category.
  name: id
  type: string
- description: Title of the category.
  name: title
  type: string
- description: Display order of the category within its parent.
  name: order
  type: integer
- description: Identifier of the parent category, if nested.
  name: parentCategoryId
  type: string
- description: Identifier of the project version containing the category.
  name: projectVersionId
  type: string
provider_name: Document360
provider_slug: document360
schema_file: json-schema/document360-category-schema.json
slug: document360-category
source_filename: document360-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/json-schema/document360-category-schema.json\",\n  \"title\": \"Document360 Category\",\n  \"description\": \"A category that organizes articles within a Document360 knowledge base project version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the category.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the category.\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Display order of the category within its parent.\"\n    },\n    \"parentCategoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent category, if nested.\"\n    },\n    \"projectVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier\
  \ of the project version containing the category.\"\n    }\n  },\n  \"required\": [\"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/json-schema/document360-category-schema.json
tags:
- Documentation
- Knowledge Base
- SaaS
title: Document360 Category
---
