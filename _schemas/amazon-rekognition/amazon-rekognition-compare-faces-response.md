---
description: CompareFacesResponse schema from Amazon Rekognition
layout: schema
name: CompareFacesResponse
properties_list:
- description: ''
  name: SourceImageFace
  type: object
- description: ''
  name: FaceMatches
  type: array
- description: ''
  name: UnmatchedFaces
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-compare-faces-response-schema.json
slug: amazon-rekognition-compare-faces-response
source_filename: amazon-rekognition-compare-faces-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-compare-faces-response-schema.json\",\n  \"title\": \"CompareFacesResponse\",\n  \"description\": \"CompareFacesResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceImageFace\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"BoundingBox\": {\n          \"$ref\": \"#/components/schemas/BoundingBox\"\n        },\n        \"Confidence\": {\n          \"type\": \"number\",\n          \"format\": \"float\"\n        }\n      }\n    },\n    \"FaceMatches\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Similarity\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"example\": 95.3\n          },\n          \"\
  Face\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"BoundingBox\": {\n                \"$ref\": \"#/components/schemas/BoundingBox\"\n              },\n              \"Confidence\": {\n                \"type\": \"number\",\n                \"format\": \"float\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"UnmatchedFaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-compare-faces-response-schema.json
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
title: CompareFacesResponse
---
