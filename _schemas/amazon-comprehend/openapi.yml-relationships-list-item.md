---
description: List of child blocks for the current block.
layout: schema
name: RelationshipsListItem
properties_list:
- description: ''
  name: Ids
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-relationships-list-item-schema.json
slug: openapi.yml-relationships-list-item
source_filename: openapi.yml-relationships-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-relationships-list-item-schema.json\",\n  \"title\": \"RelationshipsListItem\",\n  \"description\": \"List of child blocks for the current block.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Identifers of the child blocks.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipType\"\n        },\n        {\n          \"description\": \"Only supported relationship is a child relationship.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-relationships-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: RelationshipsListItem
---
