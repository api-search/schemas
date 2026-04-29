---
description: A Retention configuration for an object.
layout: schema
name: ObjectLockRetention
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: RetainUntilDate
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectlockretention-schema.json
slug: s3-objectlockretention
source_filename: s3-objectlockretention-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectLockRetention\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {},\n    \"RetainUntilDate\": {}\n  },\n  \"description\": \"A Retention configuration for an object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectlockretention-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectLockRetention
---
