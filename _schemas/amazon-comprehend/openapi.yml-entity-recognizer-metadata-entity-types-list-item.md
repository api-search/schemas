---
description: Individual item from the list of entity types in the metadata of an entity recognizer.
layout: schema
name: EntityRecognizerMetadataEntityTypesListItem
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: EvaluationMetrics
  type: object
- description: ''
  name: NumberOfTrainMentions
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-metadata-entity-types-list-item-schema.json
slug: openapi.yml-entity-recognizer-metadata-entity-types-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-metadata-entity-types-list-item-schema.json\",\n  \"title\": \"EntityRecognizerMetadataEntityTypesListItem\",\n  \"description\": \"Individual item from the list of entity types in the metadata of an entity recognizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"Type of entity from the list of entity types in the metadata of an entity recognizer. \"\n        }\n      ]\n    },\n    \"EvaluationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityTypesEvaluationMetrics\"\n        },\n        {\n          \"description\": \"Detailed information about the accuracy of the\
  \ entity recognizer for a specific item on the list of entity types. \"\n        }\n      ]\n    },\n    \"NumberOfTrainMentions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Indicates the number of times the given entity type was seen in the training data. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-metadata-entity-types-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerMetadataEntityTypesListItem
---
