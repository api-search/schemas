---
description: The location of the S3 bucket that contains a revision.
layout: schema
name: S3ArtifactLocation
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: objectKey
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-s3-artifact-location-schema.json
slug: amazon-codepipeline-s3-artifact-location
source_filename: amazon-codepipeline-s3-artifact-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-s3-artifact-location-schema.json\",\n  \"title\": \"S3ArtifactLocation\",\n  \"description\": \"The location of the S3 bucket that contains a revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"objectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"The key of the object in the S3 bucket, which uniquely identifies the object in the bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\",\n    \"objectKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-s3-artifact-location-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: S3ArtifactLocation
---
