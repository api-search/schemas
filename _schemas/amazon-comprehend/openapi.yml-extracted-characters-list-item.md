---
description: Array of the number of characters extracted from each page.
layout: schema
name: ExtractedCharactersListItem
properties_list:
- description: ''
  name: Page
  type: object
- description: ''
  name: Count
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-extracted-characters-list-item-schema.json
slug: openapi.yml-extracted-characters-list-item
source_filename: openapi.yml-extracted-characters-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-extracted-characters-list-item-schema.json\",\n  \"title\": \"ExtractedCharactersListItem\",\n  \"description\": \"Array of the number of characters extracted from each page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Page\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Page number.\"\n        }\n      ]\n    },\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of characters extracted from each page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-extracted-characters-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ExtractedCharactersListItem
---
