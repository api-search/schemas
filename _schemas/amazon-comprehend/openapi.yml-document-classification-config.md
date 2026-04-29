---
description: Configuration required for a custom classification model.
layout: schema
name: DocumentClassificationConfig
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: Labels
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classification-config-schema.json
slug: openapi.yml-document-classification-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classification-config-schema.json\",\n  \"title\": \"DocumentClassificationConfig\",\n  \"description\": \"Configuration required for a custom classification model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierMode\"\n        },\n        {\n          \"description\": \"Classification mode indicates whether the documents are <code>MULTI_CLASS</code> or <code>MULTI_LABEL</code>.\"\n        }\n      ]\n    },\n    \"Labels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LabelsList\"\n        },\n        {\n          \"description\": \"One or more labels to associate with the custom classifier.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Mode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classification-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassificationConfig
---
