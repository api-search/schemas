---
description: SearchFacesByImageResponse schema from Amazon Rekognition
layout: schema
name: SearchFacesByImageResponse
properties_list:
- description: ''
  name: SearchedFaceBoundingBox
  type: object
- description: ''
  name: SearchedFaceConfidence
  type: number
- description: ''
  name: FaceMatches
  type: array
- description: ''
  name: FaceModelVersion
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-search-faces-by-image-response-schema.json
slug: amazon-rekognition-search-faces-by-image-response
source_filename: amazon-rekognition-search-faces-by-image-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-search-faces-by-image-response-schema.json\",\n  \"title\": \"SearchFacesByImageResponse\",\n  \"description\": \"SearchFacesByImageResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SearchedFaceBoundingBox\": {\n      \"$ref\": \"#/components/schemas/BoundingBox\"\n    },\n    \"SearchedFaceConfidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\"\n    },\n    \"FaceMatches\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"FaceModelVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-search-faces-by-image-response-schema.json
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
title: SearchFacesByImageResponse
---
