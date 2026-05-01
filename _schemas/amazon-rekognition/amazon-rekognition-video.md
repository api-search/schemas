---
description: Video file stored in an Amazon S3 bucket.
layout: schema
name: Video
properties_list:
- description: ''
  name: S3Object
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-video-schema.json
slug: amazon-rekognition-video
source_filename: amazon-rekognition-video-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-video-schema.json\",\n  \"title\": \"Video\",\n  \"description\": \"Video file stored in an Amazon S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Object\": {\n      \"$ref\": \"#/components/schemas/S3Object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-video-schema.json
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
title: Video
---
