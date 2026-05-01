---
description: GetLabelDetectionResponse schema from Amazon Rekognition
layout: schema
name: GetLabelDetectionResponse
properties_list:
- description: ''
  name: JobStatus
  type: string
- description: ''
  name: StatusMessage
  type: string
- description: ''
  name: VideoMetadata
  type: object
- description: ''
  name: NextToken
  type: string
- description: ''
  name: Labels
  type: array
- description: ''
  name: LabelModelVersion
  type: string
- description: ''
  name: JobId
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-get-label-detection-response-schema.json
slug: amazon-rekognition-get-label-detection-response
source_filename: amazon-rekognition-get-label-detection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-label-detection-response-schema.json\",\n  \"title\": \"GetLabelDetectionResponse\",\n  \"description\": \"GetLabelDetectionResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"SUCCEEDED\",\n        \"FAILED\"\n      ],\n      \"example\": \"SUCCEEDED\"\n    },\n    \"StatusMessage\": {\n      \"type\": \"string\"\n    },\n    \"VideoMetadata\": {\n      \"type\": \"object\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"Labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Timestamp\": {\n            \"type\": \"integer\"\n          },\n\
  \          \"Label\": {\n            \"$ref\": \"#/components/schemas/Label\"\n          }\n        }\n      }\n    },\n    \"LabelModelVersion\": {\n      \"type\": \"string\"\n    },\n    \"JobId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-label-detection-response-schema.json
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
title: GetLabelDetectionResponse
---
