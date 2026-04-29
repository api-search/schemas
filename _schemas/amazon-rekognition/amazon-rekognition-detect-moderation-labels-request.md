---
description: DetectModerationLabelsRequest schema from Amazon Rekognition
layout: schema
name: DetectModerationLabelsRequest
properties_list:
- description: ''
  name: Image
  type: object
- description: Minimum confidence level for labels to return.
  name: MinConfidence
  type: number
- description: Sets up the flow for A2I human review of moderation labels.
  name: HumanLoopConfig
  type: object
- description: Identifier for a custom label detection project version.
  name: ProjectVersion
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-moderation-labels-request-schema.json
slug: amazon-rekognition-detect-moderation-labels-request
source_filename: amazon-rekognition-detect-moderation-labels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-moderation-labels-request-schema.json\",\n  \"title\": \"DetectModerationLabelsRequest\",\n  \"description\": \"DetectModerationLabelsRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"MinConfidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Minimum confidence level for labels to return.\",\n      \"example\": 50.0\n    },\n    \"HumanLoopConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Sets up the flow for A2I human review of moderation labels.\"\n    },\n    \"ProjectVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for a custom label detection project version.\"\n\
  \    }\n  },\n  \"required\": [\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-moderation-labels-request-schema.json
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
title: DetectModerationLabelsRequest
---
