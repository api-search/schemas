---
description: DetectCustomLabelsRequest schema from Amazon Rekognition
layout: schema
name: DetectCustomLabelsRequest
properties_list:
- description: The ARN of the model version to use.
  name: ProjectVersionArn
  type: string
- description: ''
  name: Image
  type: object
- description: ''
  name: MaxResults
  type: integer
- description: ''
  name: MinConfidence
  type: number
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-custom-labels-request-schema.json
slug: amazon-rekognition-detect-custom-labels-request
source_filename: amazon-rekognition-detect-custom-labels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-custom-labels-request-schema.json\",\n  \"title\": \"DetectCustomLabelsRequest\",\n  \"description\": \"DetectCustomLabelsRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectVersionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the model version to use.\"\n    },\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\"\n    },\n    \"MinConfidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\"\n    }\n  },\n  \"required\": [\n    \"ProjectVersionArn\",\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-custom-labels-request-schema.json
tags:
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
title: DetectCustomLabelsRequest
---
