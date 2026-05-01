---
description: StartLabelDetectionRequest schema from Amazon Rekognition
layout: schema
name: StartLabelDetectionRequest
properties_list:
- description: ''
  name: Video
  type: object
- description: ''
  name: ClientRequestToken
  type: string
- description: ''
  name: MinConfidence
  type: number
- description: ''
  name: NotificationChannel
  type: object
- description: ''
  name: JobTag
  type: string
- description: ''
  name: Features
  type: array
- description: ''
  name: Settings
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-start-label-detection-request-schema.json
slug: amazon-rekognition-start-label-detection-request
source_filename: amazon-rekognition-start-label-detection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-start-label-detection-request-schema.json\",\n  \"title\": \"StartLabelDetectionRequest\",\n  \"description\": \"StartLabelDetectionRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Video\": {\n      \"$ref\": \"#/components/schemas/Video\"\n    },\n    \"ClientRequestToken\": {\n      \"type\": \"string\"\n    },\n    \"MinConfidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 75.0\n    },\n    \"NotificationChannel\": {\n      \"$ref\": \"#/components/schemas/NotificationChannel\"\n    },\n    \"JobTag\": {\n      \"type\": \"string\"\n    },\n    \"Features\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"Settings\": {\n      \"type\": \"\
  object\"\n    }\n  },\n  \"required\": [\n    \"Video\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-start-label-detection-request-schema.json
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
title: StartLabelDetectionRequest
---
