---
description: IndexFacesRequest schema from Amazon Rekognition
layout: schema
name: IndexFacesRequest
properties_list:
- description: ''
  name: CollectionId
  type: string
- description: ''
  name: Image
  type: object
- description: ID you want to assign to all faces detected in the image.
  name: ExternalImageId
  type: string
- description: ''
  name: DetectionAttributes
  type: array
- description: Maximum number of faces to index.
  name: MaxFaces
  type: integer
- description: ''
  name: QualityFilter
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-index-faces-request-schema.json
slug: amazon-rekognition-index-faces-request
source_filename: amazon-rekognition-index-faces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-index-faces-request-schema.json\",\n  \"title\": \"IndexFacesRequest\",\n  \"description\": \"IndexFacesRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CollectionId\": {\n      \"type\": \"string\",\n      \"example\": \"my-face-collection\"\n    },\n    \"Image\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"ExternalImageId\": {\n      \"type\": \"string\",\n      \"description\": \"ID you want to assign to all faces detected in the image.\",\n      \"example\": \"user-123\"\n    },\n    \"DetectionAttributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"DEFAULT\",\n          \"ALL\"\n        ]\n      }\n    },\n    \"MaxFaces\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Maximum number of faces to index.\"\n    },\n    \"QualityFilter\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"AUTO\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ]\n    }\n  },\n  \"required\": [\n    \"CollectionId\",\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-index-faces-request-schema.json
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
title: IndexFacesRequest
---
