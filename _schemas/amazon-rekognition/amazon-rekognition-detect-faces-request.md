---
description: DetectFacesRequest schema from Amazon Rekognition
layout: schema
name: DetectFacesRequest
properties_list:
- description: ''
  name: Image
  type: object
- description: An array of facial attributes to return. ALL returns all attributes.
  name: Attributes
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-faces-request-schema.json
slug: amazon-rekognition-detect-faces-request
source_filename: amazon-rekognition-detect-faces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-faces-request-schema.json\",\n  \"title\": \"DetectFacesRequest\",\n  \"description\": \"DetectFacesRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"Attributes\": {\n      \"type\": \"array\",\n      \"description\": \"An array of facial attributes to return. ALL returns all attributes.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"DEFAULT\",\n          \"ALL\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-faces-request-schema.json
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
title: DetectFacesRequest
---
