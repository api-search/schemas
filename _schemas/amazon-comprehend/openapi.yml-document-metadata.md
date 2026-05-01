---
description: Information about the document, discovered during text extraction.
layout: schema
name: DocumentMetadata
properties_list:
- description: ''
  name: Pages
  type: object
- description: ''
  name: ExtractedCharacters
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-metadata-schema.json
slug: openapi.yml-document-metadata
source_filename: openapi.yml-document-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-metadata-schema.json\",\n  \"title\": \"DocumentMetadata\",\n  \"description\": \"Information about the document, discovered during text extraction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of pages in the document.\"\n        }\n      ]\n    },\n    \"ExtractedCharacters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfExtractedCharacters\"\n        },\n        {\n          \"description\": \"List of pages in the document, with the number of characters extracted from each page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-metadata-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentMetadata
---
