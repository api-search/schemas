---
description: GetVideoJobResultRequest schema from Amazon Rekognition
layout: schema
name: GetVideoJobResultRequest
properties_list:
- description: Job identifier from the start job call.
  name: JobId
  type: string
- description: ''
  name: MaxResults
  type: integer
- description: ''
  name: NextToken
  type: string
- description: ''
  name: SortBy
  type: string
- description: ''
  name: AggregateBy
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-get-video-job-result-request-schema.json
slug: amazon-rekognition-get-video-job-result-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-video-job-result-request-schema.json\",\n  \"title\": \"GetVideoJobResultRequest\",\n  \"description\": \"GetVideoJobResultRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job identifier from the start job call.\",\n      \"example\": \"1234567890abcdef\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"SortBy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NAME\",\n        \"TIMESTAMP\"\n      ]\n    },\n    \"AggregateBy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TIMESTAMPS\",\n        \"SEGMENTS\"\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-get-video-job-result-request-schema.json
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
title: GetVideoJobResultRequest
---
