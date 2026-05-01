---
description: The S3 location where Amazon Lookout for Vision saves training output.
layout: schema
name: OutputS3Object
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Key
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-output-s3-object-schema.json
slug: amazon-lookout-for-vision-output-s3-object
source_filename: amazon-lookout-for-vision-output-s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-output-s3-object-schema.json\",\n  \"title\": \"OutputS3Object\",\n  \"description\": \"The S3 location where Amazon Lookout for Vision saves training output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The bucket that contains the training output.\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The location of the training output in the bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Bucket\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-output-s3-object-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: OutputS3Object
---
