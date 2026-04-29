---
description: Request for the DetectLabels operation.
layout: schema
name: DetectLabelsRequest
properties_list:
- description: ''
  name: Image
  type: object
- description: Maximum number of labels to return.
  name: MaxLabels
  type: integer
- description: Minimum confidence level for labels to return.
  name: MinConfidence
  type: number
- description: A list of the types of analysis to perform.
  name: Features
  type: array
- description: Optional settings for label detection.
  name: Settings
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-labels-request-schema.json
slug: amazon-rekognition-detect-labels-request
source_filename: amazon-rekognition-detect-labels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-labels-request-schema.json\",\n  \"title\": \"DetectLabelsRequest\",\n  \"description\": \"Request for the DetectLabels operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"MaxLabels\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of labels to return.\",\n      \"example\": 10\n    },\n    \"MinConfidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Minimum confidence level for labels to return.\",\n      \"example\": 75.0\n    },\n    \"Features\": {\n      \"type\": \"array\",\n      \"description\": \"A list of the types of analysis to perform.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\"\
  : [\n          \"GENERAL_LABELS\",\n          \"IMAGE_PROPERTIES\"\n        ]\n      }\n    },\n    \"Settings\": {\n      \"type\": \"object\",\n      \"description\": \"Optional settings for label detection.\"\n    }\n  },\n  \"required\": [\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-labels-request-schema.json
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
title: DetectLabelsRequest
---
