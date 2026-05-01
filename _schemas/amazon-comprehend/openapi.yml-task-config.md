---
description: Configuration about the custom classifier associated with the flywheel.
layout: schema
name: TaskConfig
properties_list:
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: DocumentClassificationConfig
  type: object
- description: ''
  name: EntityRecognitionConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-task-config-schema.json
slug: openapi.yml-task-config
source_filename: openapi.yml-task-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-task-config-schema.json\",\n  \"title\": \"TaskConfig\",\n  \"description\": \"Configuration about the custom classifier associated with the flywheel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"Language code for the language that the model supports.\"\n        }\n      ]\n    },\n    \"DocumentClassificationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassificationConfig\"\n        },\n        {\n          \"description\": \"Configuration required for a classification model.\"\n        }\n      ]\n    },\n    \"EntityRecognitionConfig\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/EntityRecognitionConfig\"\n        },\n        {\n          \"description\": \"Configuration required for an entity recognition model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-task-config-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: TaskConfig
---
