---
description: Specifies one of the label or labels that categorize the document being analyzed.
layout: schema
name: DocumentLabel
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Score
  type: object
- description: ''
  name: Page
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-label-schema.json
slug: openapi.yml-document-label
source_filename: openapi.yml-document-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-label-schema.json\",\n  \"title\": \"DocumentLabel\",\n  \"description\": \"Specifies one of the label or labels that categorize the document being analyzed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the label.\"\n        }\n      ]\n    },\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The confidence score that Amazon Comprehend has this label correctly attributed.\"\n        }\n      ]\n    },\n    \"Page\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n       \
  \ },\n        {\n          \"description\": \"Page number where the label occurs. This field is present in the response only if your request includes the <code>Byte</code> parameter. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-label-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentLabel
---
