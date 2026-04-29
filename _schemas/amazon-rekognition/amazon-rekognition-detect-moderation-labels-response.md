---
description: DetectModerationLabelsResponse schema from Amazon Rekognition
layout: schema
name: DetectModerationLabelsResponse
properties_list:
- description: ''
  name: ModerationLabels
  type: array
- description: ''
  name: ModerationModelVersion
  type: string
- description: ''
  name: HumanLoopActivationOutput
  type: object
- description: ''
  name: ProjectVersion
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-moderation-labels-response-schema.json
slug: amazon-rekognition-detect-moderation-labels-response
source_filename: amazon-rekognition-detect-moderation-labels-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-moderation-labels-response-schema.json\",\n  \"title\": \"DetectModerationLabelsResponse\",\n  \"description\": \"DetectModerationLabelsResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModerationLabels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"Explicit Nudity\"\n          },\n          \"ParentName\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"ModerationModelVersion\": {\n      \"type\": \"string\",\n      \"example\": \"7.0\"\
  \n    },\n    \"HumanLoopActivationOutput\": {\n      \"type\": \"object\"\n    },\n    \"ProjectVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-moderation-labels-response-schema.json
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
title: DetectModerationLabelsResponse
---
