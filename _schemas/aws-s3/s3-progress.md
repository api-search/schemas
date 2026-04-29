---
description: This data type contains information about progress of an operation.
layout: schema
name: Progress
properties_list:
- description: ''
  name: BytesScanned
  type: object
- description: ''
  name: BytesProcessed
  type: object
- description: ''
  name: BytesReturned
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-progress-schema.json
slug: s3-progress
source_filename: s3-progress-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Progress\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BytesScanned\": {},\n    \"BytesProcessed\": {},\n    \"BytesReturned\": {}\n  },\n  \"description\": \"This data type contains information about progress of an operation.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-progress-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Progress
---
