---
description: CreateCollectionResponse schema from Amazon Rekognition
layout: schema
name: CreateCollectionResponse
properties_list:
- description: ''
  name: StatusCode
  type: integer
- description: ''
  name: CollectionArn
  type: string
- description: ''
  name: FaceModelVersion
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-create-collection-response-schema.json
slug: amazon-rekognition-create-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-create-collection-response-schema.json\",\n  \"title\": \"CreateCollectionResponse\",\n  \"description\": \"CreateCollectionResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StatusCode\": {\n      \"type\": \"integer\",\n      \"example\": 200\n    },\n    \"CollectionArn\": {\n      \"type\": \"string\",\n      \"example\": \"aws:rekognition:us-east-1:123456789012:collection/my-face-collection\"\n    },\n    \"FaceModelVersion\": {\n      \"type\": \"string\",\n      \"example\": \"6.0\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-create-collection-response-schema.json
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
title: CreateCollectionResponse
---
