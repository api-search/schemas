---
description: Container for all response elements.
layout: schema
name: CopyPartResult
properties_list:
- description: ''
  name: ETag
  type: object
- description: ''
  name: LastModified
  type: object
- description: ''
  name: ChecksumCRC32
  type: object
- description: ''
  name: ChecksumCRC32C
  type: object
- description: ''
  name: ChecksumSHA1
  type: object
- description: ''
  name: ChecksumSHA256
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-copypartresult-schema.json
slug: s3-copypartresult
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopyPartResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ETag\": {},\n    \"LastModified\": {},\n    \"ChecksumCRC32\": {},\n    \"ChecksumCRC32C\": {},\n    \"ChecksumSHA1\": {},\n    \"ChecksumSHA256\": {}\n  },\n  \"description\": \"Container for all response elements.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-copypartresult-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CopyPartResult
---
