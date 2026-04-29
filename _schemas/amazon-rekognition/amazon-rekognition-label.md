---
description: Structure containing details about the detected label.
layout: schema
name: Label
properties_list:
- description: The name of the label detected in the image or video.
  name: Name
  type: string
- description: Level of confidence for the label.
  name: Confidence
  type: number
- description: Bounding boxes for each instance of the detected object.
  name: Instances
  type: array
- description: The parent labels for a label in the taxonomy hierarchy.
  name: Parents
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-label-schema.json
slug: amazon-rekognition-label
source_filename: amazon-rekognition-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-label-schema.json\",\n  \"title\": \"Label\",\n  \"description\": \"Structure containing details about the detected label.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the label detected in the image or video.\",\n      \"example\": \"Person\"\n    },\n    \"Confidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Level of confidence for the label.\",\n      \"example\": 98.5\n    },\n    \"Instances\": {\n      \"type\": \"array\",\n      \"description\": \"Bounding boxes for each instance of the detected object.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"BoundingBox\": {\n            \"$ref\": \"#/components/schemas/BoundingBox\"\
  \n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\n          }\n        }\n      }\n    },\n    \"Parents\": {\n      \"type\": \"array\",\n      \"description\": \"The parent labels for a label in the taxonomy hierarchy.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-label-schema.json
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
title: Label
---
