---
description: Amazon S3 Location information for an input manifest file.
layout: schema
name: InputS3Object
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-input-s3-object-schema.json
slug: amazon-lookout-for-vision-input-s3-object
source_filename: amazon-lookout-for-vision-input-s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-input-s3-object-schema.json\",\n  \"title\": \"InputS3Object\",\n  \"description\": \"Amazon S3 Location information for an input manifest file. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket that contains the manifest.\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The name and location of the manifest file withiin the bucket.\"\n        }\n      ]\n    },\n    \"VersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectVersion\"\
  \n        },\n        {\n          \"description\": \"The version ID of the bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Bucket\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-input-s3-object-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: InputS3Object
---
