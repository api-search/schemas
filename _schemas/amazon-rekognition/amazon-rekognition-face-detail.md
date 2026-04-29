---
description: Structure containing attributes of the face that the algorithm detected.
layout: schema
name: FaceDetail
properties_list:
- description: ''
  name: BoundingBox
  type: object
- description: The estimated age range in years for the face.
  name: AgeRange
  type: object
- description: ''
  name: Smile
  type: object
- description: ''
  name: Gender
  type: object
- description: ''
  name: Emotions
  type: array
- description: Confidence level that the bounding box contains a face.
  name: Confidence
  type: number
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-face-detail-schema.json
slug: amazon-rekognition-face-detail
source_filename: amazon-rekognition-face-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-face-detail-schema.json\",\n  \"title\": \"FaceDetail\",\n  \"description\": \"Structure containing attributes of the face that the algorithm detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BoundingBox\": {\n      \"$ref\": \"#/components/schemas/BoundingBox\"\n    },\n    \"AgeRange\": {\n      \"type\": \"object\",\n      \"description\": \"The estimated age range in years for the face.\",\n      \"properties\": {\n        \"Low\": {\n          \"type\": \"integer\",\n          \"example\": 25\n        },\n        \"High\": {\n          \"type\": \"integer\",\n          \"example\": 35\n        }\n      }\n    },\n    \"Smile\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Value\": {\n          \"type\": \"boolean\"\n        },\n        \"\
  Confidence\": {\n          \"type\": \"number\",\n          \"format\": \"float\"\n        }\n      }\n    },\n    \"Gender\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Value\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Male\",\n            \"Female\"\n          ]\n        },\n        \"Confidence\": {\n          \"type\": \"number\",\n          \"format\": \"float\"\n        }\n      }\n    },\n    \"Emotions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HAPPY\",\n              \"SAD\",\n              \"ANGRY\",\n              \"CONFUSED\",\n              \"DISGUSTED\",\n              \"SURPRISED\",\n              \"CALM\",\n              \"UNKNOWN\",\n              \"FEAR\"\n            ]\n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n\
  \            \"format\": \"float\"\n          }\n        }\n      }\n    },\n    \"Confidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Confidence level that the bounding box contains a face.\",\n      \"example\": 99.7\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-face-detail-schema.json
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
title: FaceDetail
---
