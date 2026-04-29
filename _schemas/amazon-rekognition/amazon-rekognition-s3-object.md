---
description: Provides the S3 bucket name and object name.
layout: schema
name: S3Object
properties_list:
- description: Name of the S3 bucket.
  name: Bucket
  type: string
- description: S3 object key name.
  name: Name
  type: string
- description: S3 object version ID if versioning is enabled.
  name: Version
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-s3-object-schema.json
slug: amazon-rekognition-s3-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-s3-object-schema.json\",\n  \"title\": \"S3Object\",\n  \"description\": \"Provides the S3 bucket name and object name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the S3 bucket.\",\n      \"example\": \"my-images-bucket\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"S3 object key name.\",\n      \"example\": \"images/photo.jpg\"\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"S3 object version ID if versioning is enabled.\",\n      \"example\": \"v1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-s3-object-schema.json
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
title: S3Object
---
