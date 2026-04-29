---
description: Document type for each page in the document.
layout: schema
name: DocumentTypeListItem
properties_list:
- description: ''
  name: Page
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-type-list-item-schema.json
slug: openapi.yml-document-type-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-type-list-item-schema.json\",\n  \"title\": \"DocumentTypeListItem\",\n  \"description\": \"Document type for each page in the document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Page\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Page number.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentType\"\n        },\n        {\n          \"description\": \"Document type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-type-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentTypeListItem
---
