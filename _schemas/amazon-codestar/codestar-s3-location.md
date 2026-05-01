---
description: The Amazon S3 location where the source code files provided with the project request are stored.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: bucketKey
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-s3-location-schema.json
slug: codestar-s3-location
source_filename: codestar-s3-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"The Amazon S3 location where the source code files provided with the project request are stored.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket name where the source code files provided with the project request are stored.\"\n        }\n      ]\n    },\n    \"bucketKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketKey\"\n        },\n        {\n          \"description\": \"The Amazon S3 object key where the source code files provided with the project request are stored.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-s3-location-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: S3Location
---
