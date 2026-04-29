---
description: Detailed information about an entity recognizer.
layout: schema
name: EntityRecognizerMetadata
properties_list:
- description: ''
  name: NumberOfTrainedDocuments
  type: object
- description: ''
  name: NumberOfTestDocuments
  type: object
- description: ''
  name: EvaluationMetrics
  type: object
- description: ''
  name: EntityTypes
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-metadata-schema.json
slug: openapi.yml-entity-recognizer-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-metadata-schema.json\",\n  \"title\": \"EntityRecognizerMetadata\",\n  \"description\": \"Detailed information about an entity recognizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumberOfTrainedDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of documents in the input data that were used to train the entity recognizer. Typically this is 80 to 90 percent of the input documents.\"\n        }\n      ]\n    },\n    \"NumberOfTestDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of documents in the input data that were used to test the\
  \ entity recognizer. Typically this is 10 to 20 percent of the input documents.\"\n        }\n      ]\n    },\n    \"EvaluationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerEvaluationMetrics\"\n        },\n        {\n          \"description\": \"Detailed information about the accuracy of an entity recognizer.\"\n        }\n      ]\n    },\n    \"EntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerMetadataEntityTypesList\"\n        },\n        {\n          \"description\": \"Entity types from the metadata of an entity recognizer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-metadata-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerMetadata
---
