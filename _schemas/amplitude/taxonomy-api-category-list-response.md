---
description: CategoryListResponse schema from Amplitude Taxonomy API
layout: schema
name: CategoryListResponse
properties_list:
- description: Array of event categories.
  name: data
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-category-list-response-schema.json
slug: taxonomy-api-category-list-response
source_filename: taxonomy-api-category-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-category-list-response-schema.json\",\n  \"title\": \"CategoryListResponse\",\n  \"description\": \"CategoryListResponse schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event categories.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier of the category.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the category.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-category-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CategoryListResponse
---
