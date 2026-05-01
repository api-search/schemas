---
description: CompareFacesRequest schema from Amazon Rekognition
layout: schema
name: CompareFacesRequest
properties_list:
- description: ''
  name: SourceImage
  type: object
- description: ''
  name: TargetImage
  type: object
- description: Minimum confidence for a match to be included in FaceMatches.
  name: SimilarityThreshold
  type: number
- description: ''
  name: QualityFilter
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-compare-faces-request-schema.json
slug: amazon-rekognition-compare-faces-request
source_filename: amazon-rekognition-compare-faces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-compare-faces-request-schema.json\",\n  \"title\": \"CompareFacesRequest\",\n  \"description\": \"CompareFacesRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceImage\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"TargetImage\": {\n      \"$ref\": \"#/components/schemas/Image\"\n    },\n    \"SimilarityThreshold\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Minimum confidence for a match to be included in FaceMatches.\",\n      \"example\": 80.0\n    },\n    \"QualityFilter\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"AUTO\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  SourceImage\",\n    \"TargetImage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-compare-faces-request-schema.json
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
title: CompareFacesRequest
---
