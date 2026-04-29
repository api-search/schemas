---
description: Describes the result metrics for the test data associated with an documentation classifier.
layout: schema
name: ClassifierEvaluationMetrics
properties_list:
- description: ''
  name: Accuracy
  type: object
- description: ''
  name: Precision
  type: object
- description: ''
  name: Recall
  type: object
- description: ''
  name: F1Score
  type: object
- description: ''
  name: MicroPrecision
  type: object
- description: ''
  name: MicroRecall
  type: object
- description: ''
  name: MicroF1Score
  type: object
- description: ''
  name: HammingLoss
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-classifier-evaluation-metrics-schema.json
slug: openapi.yml-classifier-evaluation-metrics
source_filename: openapi.yml-classifier-evaluation-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classifier-evaluation-metrics-schema.json\",\n  \"title\": \"ClassifierEvaluationMetrics\",\n  \"description\": \"Describes the result metrics for the test data associated with an documentation classifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accuracy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The fraction of the labels that were correct recognized. It is computed by dividing the number of labels in the test documents that were correctly recognized by the total number of labels in the test documents.\"\n        }\n      ]\n    },\n    \"Precision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\"\
  : \"A measure of the usefulness of the classifier results in the test data. High precision means that the classifier returned substantially more relevant results than irrelevant ones.\"\n        }\n      ]\n    },\n    \"Recall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of how complete the classifier results are for the test data. High recall means that the classifier returned most of the relevant results. \"\n        }\n      ]\n    },\n    \"F1Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of how accurate the classifier results are for the test data. It is derived from the <code>Precision</code> and <code>Recall</code> values. The <code>F1Score</code> is the harmonic average of the two scores. The highest score is 1, and the worst score is 0. \"\n        }\n      ]\n\
  \    },\n    \"MicroPrecision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of the usefulness of the recognizer results in the test data. High precision means that the recognizer returned substantially more relevant results than irrelevant ones. Unlike the Precision metric which comes from averaging the precision of all available labels, this is based on the overall score of all precision scores added together.\"\n        }\n      ]\n    },\n    \"MicroRecall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of how complete the classifier results are for the test data. High recall means that the classifier returned most of the relevant results. Specifically, this indicates how many of the correct categories in the text that the model can predict. It is a percentage of correct categories\
  \ in the text that can found. Instead of averaging the recall scores of all labels (as with Recall), micro Recall is based on the overall score of all recall scores added together.\"\n        }\n      ]\n    },\n    \"MicroF1Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A measure of how accurate the classifier results are for the test data. It is a combination of the <code>Micro Precision</code> and <code>Micro Recall</code> values. The <code>Micro F1Score</code> is the harmonic mean of the two scores. The highest score is 1, and the worst score is 0.\"\n        }\n      ]\n    },\n    \"HammingLoss\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Indicates the fraction of labels that are incorrectly predicted. Also seen as the fraction of wrong labels compared to the total number of labels. Scores\
  \ closer to zero are better.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classifier-evaluation-metrics-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ClassifierEvaluationMetrics
---
