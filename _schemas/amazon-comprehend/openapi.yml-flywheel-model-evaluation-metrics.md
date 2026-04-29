---
description: The evaluation metrics associated with the evaluated model.
layout: schema
name: FlywheelModelEvaluationMetrics
properties_list:
- description: ''
  name: AverageF1Score
  type: object
- description: ''
  name: AveragePrecision
  type: object
- description: ''
  name: AverageRecall
  type: object
- description: ''
  name: AverageAccuracy
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-flywheel-model-evaluation-metrics-schema.json
slug: openapi.yml-flywheel-model-evaluation-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-model-evaluation-metrics-schema.json\",\n  \"title\": \"FlywheelModelEvaluationMetrics\",\n  \"description\": \"The evaluation metrics associated with the evaluated model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AverageF1Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The average F1 score from the evaluation metrics.\"\n        }\n      ]\n    },\n    \"AveragePrecision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Average precision metric for the model.\"\n        }\n      ]\n    },\n    \"AverageRecall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\
  \n        },\n        {\n          \"description\": \"Average recall metric for the model.\"\n        }\n      ]\n    },\n    \"AverageAccuracy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Average accuracy metric for the model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-model-evaluation-metrics-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: FlywheelModelEvaluationMetrics
---
