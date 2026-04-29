---
description: The container element for Object Lock configuration parameters.
layout: schema
name: ObjectLockConfiguration
properties_list:
- description: ''
  name: ObjectLockEnabled
  type: object
- description: ''
  name: Rule
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectlockconfiguration-schema.json
slug: s3-objectlockconfiguration
source_filename: s3-objectlockconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectLockConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectLockEnabled\": {},\n    \"Rule\": {}\n  },\n  \"description\": \"The container element for Object Lock configuration parameters.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectlockconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectLockConfiguration
---
