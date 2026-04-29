---
description: DetectTextResponse schema from Amazon Rekognition
layout: schema
name: DetectTextResponse
properties_list:
- description: An array of text detected in the input image.
  name: TextDetections
  type: array
- description: ''
  name: TextModelVersion
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-text-response-schema.json
slug: amazon-rekognition-detect-text-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-text-response-schema.json\",\n  \"title\": \"DetectTextResponse\",\n  \"description\": \"DetectTextResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextDetections\": {\n      \"type\": \"array\",\n      \"description\": \"An array of text detected in the input image.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DetectedText\": {\n            \"type\": \"string\",\n            \"example\": \"Hello World\"\n          },\n          \"Type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"LINE\",\n              \"WORD\"\n            ]\n          },\n          \"Id\": {\n            \"type\": \"integer\"\n          },\n          \"ParentId\": {\n      \
  \      \"type\": \"integer\"\n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\n          },\n          \"Geometry\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"BoundingBox\": {\n                \"$ref\": \"#/components/schemas/BoundingBox\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"TextModelVersion\": {\n      \"type\": \"string\",\n      \"example\": \"3.1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-text-response-schema.json
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
title: DetectTextResponse
---
