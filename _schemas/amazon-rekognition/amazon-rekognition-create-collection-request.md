---
description: CreateCollectionRequest schema from Amazon Rekognition
layout: schema
name: CreateCollectionRequest
properties_list:
- description: ID for the collection to create.
  name: CollectionId
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-create-collection-request-schema.json
slug: amazon-rekognition-create-collection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-create-collection-request-schema.json\",\n  \"title\": \"CreateCollectionRequest\",\n  \"description\": \"CreateCollectionRequest schema from Amazon Rekognition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CollectionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID for the collection to create.\",\n      \"example\": \"my-face-collection\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"CollectionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-create-collection-request-schema.json
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
title: CreateCollectionRequest
---
