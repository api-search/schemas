---
description: Provides information about a document classifier.
layout: schema
name: ClassifierMetadata
properties_list:
- description: ''
  name: NumberOfLabels
  type: object
- description: ''
  name: NumberOfTrainedDocuments
  type: object
- description: ''
  name: NumberOfTestDocuments
  type: object
- description: ''
  name: EvaluationMetrics
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-classifier-metadata-schema.json
slug: openapi.yml-classifier-metadata
source_filename: openapi.yml-classifier-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classifier-metadata-schema.json\",\n  \"title\": \"ClassifierMetadata\",\n  \"description\": \"Provides information about a document classifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumberOfLabels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of labels in the input data. \"\n        }\n      ]\n    },\n    \"NumberOfTrainedDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of documents in the input data that were used to train the classifier. Typically this is 80 to 90 percent of the input documents.\"\n        }\n      ]\n    },\n    \"NumberOfTestDocuments\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of documents in the input data that were used to test the classifier. Typically this is 10 to 20 percent of the input documents, up to 10,000 documents.\"\n        }\n      ]\n    },\n    \"EvaluationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassifierEvaluationMetrics\"\n        },\n        {\n          \"description\": \" Describes the result metrics for the test data associated with an documentation classifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classifier-metadata-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ClassifierMetadata
---
