---
description: DetectFacesResponse schema from Amazon Rekognition
layout: schema
name: DetectFacesResponse
properties_list:
- description: Details of each face found in the image.
  name: FaceDetails
  type: array
- description: Orientation correction value.
  name: OrientationCorrection
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-faces-response-schema.json
slug: amazon-rekognition-detect-faces-response
source_filename: amazon-rekognition-detect-faces-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-faces-response-schema.json\",\n  \"title\": \"DetectFacesResponse\",\n  \"description\": \"DetectFacesResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FaceDetails\": {\n      \"type\": \"array\",\n      \"description\": \"Details of each face found in the image.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FaceDetail\"\n      }\n    },\n    \"OrientationCorrection\": {\n      \"type\": \"string\",\n      \"description\": \"Orientation correction value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-faces-response-schema.json
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
title: DetectFacesResponse
---
