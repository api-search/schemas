---
description: Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versioning enabled (or suspended) to request that Amazon S3 delete noncurrent object versions at a specific period in the object's lifetime.
layout: schema
name: NoncurrentVersionExpiration
properties_list:
- description: ''
  name: NoncurrentDays
  type: object
- description: ''
  name: NewerNoncurrentVersions
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-noncurrentversionexpiration-schema.json
slug: s3-noncurrentversionexpiration
source_filename: s3-noncurrentversionexpiration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoncurrentVersionExpiration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NoncurrentDays\": {},\n    \"NewerNoncurrentVersions\": {}\n  },\n  \"description\": \"Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versioning enabled (or suspended) to request that Amazon S3 delete noncurrent object versions at a specific period in the object's lifetime.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-noncurrentversionexpiration-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: NoncurrentVersionExpiration
---
