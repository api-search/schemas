---
description: ''
layout: schema
name: CreateAccessPointRequest
properties_list:
- description: The name of the bucket you want to associate with the access point.
  name: Bucket
  type: string
- description: ''
  name: VpcConfiguration
  type: object
- description: The AWS account ID associated with the S3 bucket.
  name: BucketAccountId
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-create-access-point-request-schema.json
slug: amazon-s3-control-create-access-point-request
source_filename: amazon-s3-control-create-access-point-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateAccessPointRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket you want to associate with the access point.\"\n    },\n    \"VpcConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"BucketAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID associated with the S3 bucket.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-create-access-point-request-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CreateAccessPointRequest
---
