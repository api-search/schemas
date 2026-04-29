---
description: Amazon S3 logging configuration.
layout: schema
name: S3Logs
properties_list:
- description: ''
  name: s3BucketName
  type: object
- description: ''
  name: s3KeyPrefix
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-s3-logs-schema.json
slug: ec2-image-builder-s3-logs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-s3-logs-schema.json\",\n  \"title\": \"S3Logs\",\n  \"description\": \"Amazon S3 logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The S3 bucket in which to store the logs.\"\n        }\n      ]\n    },\n    \"s3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon S3 path to the bucket where the logs are stored.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-s3-logs-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: S3Logs
---
