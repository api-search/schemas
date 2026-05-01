---
description: A location in Amazon S3.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: ObjectKey
  type: object
- description: ''
  name: Region
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-s3-location-schema.json
slug: openapi-s3-location
source_filename: openapi-s3-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"A location in Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"A bucket name.\"\n        }\n      ]\n    },\n    \"ObjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectKey\"\n        },\n        {\n          \"description\": \"An object key.\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The bucket's Region.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"BucketName\",\n    \"ObjectKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-s3-location-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: S3Location
---
