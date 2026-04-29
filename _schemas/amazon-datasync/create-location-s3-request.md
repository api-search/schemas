---
description: Request body for creating an Amazon S3 location.
layout: schema
name: Create Location S3 Request
properties_list:
- description: The ARN of the S3 bucket. This ARN uniquely identifies the bucket.
  name: S3BucketArn
  type: string
- description: ''
  name: S3StorageClass
  type: string
- description: ''
  name: Subdirectory
  type: string
- description: ''
  name: S3Config
  type: object
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/create-location-s3-request-schema.json
slug: create-location-s3-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/create-location-s3-request-schema.json\",\n  \"title\": \"Create Location S3 Request\",\n  \"description\": \"Request body for creating an Amazon S3 location.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"S3BucketArn\",\n    \"S3Config\"\n  ],\n  \"properties\": {\n    \"S3BucketArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the S3 bucket. This ARN uniquely identifies the bucket.\"\n    },\n    \"S3StorageClass\": {\n      \"type\": \"string\"\n    },\n    \"Subdirectory\": {\n      \"type\": \"string\"\n    },\n    \"S3Config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/create-location-s3-request-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Create Location S3 Request
---
