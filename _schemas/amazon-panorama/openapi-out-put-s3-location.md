---
description: The location of an output object in Amazon S3.
layout: schema
name: OutPutS3Location
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: ObjectKey
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-out-put-s3-location-schema.json
slug: openapi-out-put-s3-location
source_filename: openapi-out-put-s3-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-out-put-s3-location-schema.json\",\n  \"title\": \"OutPutS3Location\",\n  \"description\": \"The location of an output object in Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The object's bucket.\"\n        }\n      ]\n    },\n    \"ObjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectKey\"\n        },\n        {\n          \"description\": \"The object's key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BucketName\",\n    \"ObjectKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-out-put-s3-location-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: OutPutS3Location
---
