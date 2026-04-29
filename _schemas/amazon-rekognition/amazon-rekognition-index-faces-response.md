---
description: IndexFacesResponse schema from Amazon Rekognition
layout: schema
name: IndexFacesResponse
properties_list:
- description: ''
  name: FaceRecords
  type: array
- description: ''
  name: OrientationCorrection
  type: string
- description: ''
  name: FaceModelVersion
  type: string
- description: ''
  name: UnindexedFaces
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-index-faces-response-schema.json
slug: amazon-rekognition-index-faces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-index-faces-response-schema.json\",\n  \"title\": \"IndexFacesResponse\",\n  \"description\": \"IndexFacesResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FaceRecords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"OrientationCorrection\": {\n      \"type\": \"string\"\n    },\n    \"FaceModelVersion\": {\n      \"type\": \"string\"\n    },\n    \"UnindexedFaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-index-faces-response-schema.json
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
title: IndexFacesResponse
---
