---
description: Category schema from Amplitude Taxonomy API
layout: schema
name: Category
properties_list:
- description: The unique identifier of the category.
  name: id
  type: integer
- description: The name of the category.
  name: name
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-category-schema.json
slug: taxonomy-api-category
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-category-schema.json\",\n  \"title\": \"Category\",\n  \"description\": \"Category schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the category.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-category-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Category
---
