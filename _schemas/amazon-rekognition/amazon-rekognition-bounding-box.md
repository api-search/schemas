---
description: Identifies the bounding box around the label, face, text or object.
layout: schema
name: BoundingBox
properties_list:
- description: Width of the bounding box as a ratio of the overall image width.
  name: Width
  type: number
- description: Height of the bounding box as a ratio of the overall image height.
  name: Height
  type: number
- description: Left coordinate of the bounding box as a ratio of overall image width.
  name: Left
  type: number
- description: Top coordinate of the bounding box as a ratio of overall image height.
  name: Top
  type: number
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-bounding-box-schema.json
slug: amazon-rekognition-bounding-box
source_filename: amazon-rekognition-bounding-box-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-bounding-box-schema.json\",\n  \"title\": \"BoundingBox\",\n  \"description\": \"Identifies the bounding box around the label, face, text or object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Width\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Width of the bounding box as a ratio of the overall image width.\",\n      \"example\": 0.35\n    },\n    \"Height\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Height of the bounding box as a ratio of the overall image height.\",\n      \"example\": 0.45\n    },\n    \"Left\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Left coordinate of the bounding box as a ratio of overall image width.\",\n    \
  \  \"example\": 0.1\n    },\n    \"Top\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Top coordinate of the bounding box as a ratio of overall image height.\",\n      \"example\": 0.05\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-bounding-box-schema.json
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
title: BoundingBox
---
