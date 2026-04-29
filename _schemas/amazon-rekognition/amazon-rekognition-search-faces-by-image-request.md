---
description: SearchFacesByImageRequest schema from Amazon Rekognition
layout: schema
name: SearchFacesByImageRequest
properties_list:
- description: ''
  name: CollectionId
  type: string
- description: ''
  name: Image
  type: object
- description: ''
  name: MaxFaces
  type: integer
- description: ''
  name: FaceMatchThreshold
  type: number
- description: ''
  name: QualityFilter
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-search-faces-by-image-request-schema.json
slug: amazon-rekognition-search-faces-by-image-request
source_filename: amazon-rekognition-search-faces-by-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-search-faces-by-image-request-schema.json\",\n  \"title\": \"SearchFacesByImageRequest\",\n  \"description\": \"SearchFacesByImageRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CollectionId\": {\n      \"type\": \"string\",\n      \"example\": \"my-face-collection\"\n    },\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"MaxFaces\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    },\n    \"FaceMatchThreshold\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 80.0\n    },\n    \"QualityFilter\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"AUTO\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"CollectionId\",\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-search-faces-by-image-request-schema.json
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
title: SearchFacesByImageRequest
---
