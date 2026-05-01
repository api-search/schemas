---
description: RecognizeCelebritiesResponse schema from Amazon Rekognition
layout: schema
name: RecognizeCelebritiesResponse
properties_list:
- description: ''
  name: CelebrityFaces
  type: array
- description: ''
  name: UnrecognizedFaces
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-recognize-celebrities-response-schema.json
slug: amazon-rekognition-recognize-celebrities-response
source_filename: amazon-rekognition-recognize-celebrities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-recognize-celebrities-response-schema.json\",\n  \"title\": \"RecognizeCelebritiesResponse\",\n  \"description\": \"RecognizeCelebritiesResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CelebrityFaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Urls\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"Jeff Bezos\"\n          },\n          \"Id\": {\n            \"type\": \"string\"\n          },\n          \"MatchConfidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\
  \n          },\n          \"KnownGender\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"UnrecognizedFaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-recognize-celebrities-response-schema.json
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
title: RecognizeCelebritiesResponse
---
