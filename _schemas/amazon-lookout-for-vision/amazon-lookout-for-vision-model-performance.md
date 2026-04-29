---
description: Information about the evaluation performance of a trained model.
layout: schema
name: ModelPerformance
properties_list:
- description: ''
  name: F1Score
  type: object
- description: ''
  name: Recall
  type: object
- description: ''
  name: Precision
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-performance-schema.json
slug: amazon-lookout-for-vision-model-performance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-performance-schema.json\",\n  \"title\": \"ModelPerformance\",\n  \"description\": \"Information about the evaluation performance of a trained model. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"F1Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The overall F1 score metric for the trained model.\"\n        }\n      ]\n    },\n    \"Recall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The overall recall metric value for the trained model. \"\n        }\n      ]\n    },\n    \"Precision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\
  \n        },\n        {\n          \"description\": \"The overall precision metric value for the trained model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-performance-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelPerformance
---
