---
description: Template bundle S3 bucket data.
layout: schema
name: S3ObjectSource
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: key
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-s3object-source-schema.json
slug: amazon-proton-s3object-source
source_filename: amazon-proton-s3object-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-s3object-source-schema.json\",\n  \"title\": \"S3ObjectSource\",\n  \"description\": \"Template bundle S3 bucket data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket that contains a template bundle.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The path to the S3 bucket that contains a template bundle.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucket\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-s3object-source-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: S3ObjectSource
---
