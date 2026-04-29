---
description: Provides the input image either as bytes or an S3 object.
layout: schema
name: Image
properties_list:
- description: Blob of image bytes up to 5 MBs.
  name: Bytes
  type: string
- description: ''
  name: S3Object
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-image-schema.json
slug: amazon-rekognition-image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-image-schema.json\",\n  \"title\": \"Image\",\n  \"description\": \"Provides the input image either as bytes or an S3 object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bytes\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"description\": \"Blob of image bytes up to 5 MBs.\"\n    },\n    \"S3Object\": {\n      \"$ref\": \"#/components/schemas/S3Object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-image-schema.json
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
title: Image
---
