---
description: Specifies the format and location of the input data. You must provide either the <code>Annotations</code> parameter or the <code>EntityList</code> parameter.
layout: schema
name: DatasetEntityRecognizerInputDataConfig
properties_list:
- description: ''
  name: Annotations
  type: object
- description: ''
  name: Documents
  type: object
- description: ''
  name: EntityList
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-entity-recognizer-input-data-config-schema.json
slug: openapi.yml-dataset-entity-recognizer-input-data-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-input-data-config-schema.json\",\n  \"title\": \"DatasetEntityRecognizerInputDataConfig\",\n  \"description\": \"Specifies the format and location of the input data. You must provide either the <code>Annotations</code> parameter or the <code>EntityList</code> parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Annotations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetEntityRecognizerAnnotations\"\n        },\n        {\n          \"description\": \"The S3 location of the annotation documents for your custom entity recognizer.\"\n        }\n      ]\n    },\n    \"Documents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetEntityRecognizerDocuments\"\n        },\n        {\n\
  \          \"description\": \"The format and location of the training documents for your custom entity recognizer.\"\n        }\n      ]\n    },\n    \"EntityList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetEntityRecognizerEntityList\"\n        },\n        {\n          \"description\": \"The S3 location of the entity list for your custom entity recognizer.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Documents\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-input-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetEntityRecognizerInputDataConfig
---
