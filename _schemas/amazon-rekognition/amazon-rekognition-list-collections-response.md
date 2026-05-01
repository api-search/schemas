---
description: ListCollectionsResponse schema from Amazon Rekognition
layout: schema
name: ListCollectionsResponse
properties_list:
- description: ''
  name: CollectionIds
  type: array
- description: ''
  name: NextToken
  type: string
- description: ''
  name: FaceModelVersions
  type: array
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-list-collections-response-schema.json
slug: amazon-rekognition-list-collections-response
source_filename: amazon-rekognition-list-collections-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-list-collections-response-schema.json\",\n  \"title\": \"ListCollectionsResponse\",\n  \"description\": \"ListCollectionsResponse schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CollectionIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"FaceModelVersions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-list-collections-response-schema.json
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
title: ListCollectionsResponse
---
