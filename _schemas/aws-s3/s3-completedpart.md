---
description: Details of the parts that were uploaded.
layout: schema
name: CompletedPart
properties_list:
- description: ''
  name: ETag
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
- description: ''
  name: PartNumber
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-completedpart-schema.json
slug: s3-completedpart
source_filename: s3-completedpart-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletedPart\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ETag\": {},\n    \"ChecksumCRC32\": {},\n    \"ChecksumCRC32C\": {},\n    \"ChecksumSHA1\": {},\n    \"ChecksumSHA256\": {},\n    \"PartNumber\": {}\n  },\n  \"description\": \"Details of the parts that were uploaded.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-completedpart-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: CompletedPart
---
