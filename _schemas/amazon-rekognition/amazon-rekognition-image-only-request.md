---
description: Request containing only an image.
layout: schema
name: ImageOnlyRequest
properties_list:
- description: ''
  name: Image
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-image-only-request-schema.json
slug: amazon-rekognition-image-only-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-image-only-request-schema.json\",\n  \"title\": \"ImageOnlyRequest\",\n  \"description\": \"Request containing only an image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    }\n  },\n  \"required\": [\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-image-only-request-schema.json
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
title: ImageOnlyRequest
---
