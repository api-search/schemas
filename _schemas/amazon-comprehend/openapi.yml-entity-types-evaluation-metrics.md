---
description: Detailed information about the accuracy of an entity recognizer for a specific entity type.
layout: schema
name: EntityTypesEvaluationMetrics
properties_list:
- description: ''
  name: Precision
  type: object
- description: ''
  name: Recall
  type: object
- description: ''
  name: F1Score
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-types-evaluation-metrics-schema.json
slug: openapi.yml-entity-types-evaluation-metrics
source_filename: openapi.yml-entity-types-evaluation-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-types-evaluation-metrics-schema.json\",\n  \"title\": \"EntityTypesEvaluationMetrics\",\n  \"description\": \"Detailed information about the accuracy of an entity recognizer for a specific entity type. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Precision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of the usefulness of the recognizer results for a specific entity type in the test data. High precision means that the recognizer returned substantially more relevant results than irrelevant ones. \"\n        }\n      ]\n    },\n    \"Recall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\"\
  : \"A measure of how complete the recognizer results are for a specific entity type in the test data. High recall means that the recognizer returned most of the relevant results.\"\n        }\n      ]\n    },\n    \"F1Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of how accurate the recognizer results are for a specific entity type in the test data. It is derived from the <code>Precision</code> and <code>Recall</code> values. The <code>F1Score</code> is the harmonic average of the two scores. The highest score is 1, and the worst score is 0. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-types-evaluation-metrics-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityTypesEvaluationMetrics
---
