---
description: Information about the location of training output or the output of a model packaging job.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Prefix
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-s3-location-schema.json
slug: amazon-lookout-for-vision-s3-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"Information about the location of training output or the output of a model packaging job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The S3 bucket that contains the training or model packaging job output. If you are training a model, the bucket must in your AWS account. If you use an S3 bucket for a model packaging job, the S3 bucket must be in the same AWS Region and AWS account in which you use AWS IoT Greengrass.\"\n        }\n      ]\n    },\n    \"Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3KeyPrefix\"\
  \n        },\n        {\n          \"description\": \"The path of the folder, within the S3 bucket, that contains the output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Bucket\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-s3-location-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: S3Location
---
