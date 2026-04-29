---
description: DetectCustomLabelsResponse schema from Amazon Rekognition
layout: schema
name: DetectCustomLabelsResponse
properties_list:
- description: ''
  name: CustomLabels
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-custom-labels-response-schema.json
slug: amazon-rekognition-detect-custom-labels-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-custom-labels-response-schema.json\",\n  \"title\": \"DetectCustomLabelsResponse\",\n  \"description\": \"DetectCustomLabelsResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomLabels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"MyProduct\"\n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"example\": 92.3\n          },\n          \"Geometry\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-custom-labels-response-schema.json
tags:
- AWS
- Celebrity Recognition
- Computer Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine Learning
- Object Detection
- Text Detection
- Video Analysis
title: DetectCustomLabelsResponse
---
