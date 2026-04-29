---
description: GetFaceLivenessSessionResultsResponse schema from Amazon Rekognition
layout: schema
name: GetFaceLivenessSessionResultsResponse
properties_list:
- description: ''
  name: SessionId
  type: string
- description: ''
  name: Status
  type: string
- description: Confidence value between 0 and 100 of live presence.
  name: Confidence
  type: number
- description: ''
  name: ReferenceImage
  type: object
- description: ''
  name: AuditImages
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-get-face-liveness-session-results-response-schema.json
slug: amazon-rekognition-get-face-liveness-session-results-response
source_filename: amazon-rekognition-get-face-liveness-session-results-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-face-liveness-session-results-response-schema.json\",\n  \"title\": \"GetFaceLivenessSessionResultsResponse\",\n  \"description\": \"GetFaceLivenessSessionResultsResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SessionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATED\",\n        \"IN_PROGRESS\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"EXPIRED\"\n      ]\n    },\n    \"Confidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Confidence value between 0 and 100 of live presence.\",\n      \"example\": 98.5\n    },\n    \"ReferenceImage\": {\n      \"type\": \"object\"\
  \n    },\n    \"AuditImages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-face-liveness-session-results-response-schema.json
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
title: GetFaceLivenessSessionResultsResponse
---
