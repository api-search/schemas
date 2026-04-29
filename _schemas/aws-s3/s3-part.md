---
description: Container for elements related to a part.
layout: schema
name: Part
properties_list:
- description: ''
  name: PartNumber
  type: object
- description: ''
  name: LastModified
  type: object
- description: ''
  name: ETag
  type: object
- description: ''
  name: Size
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
schema_file: json-schema/s3-part-schema.json
slug: s3-part
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Part\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PartNumber\": {},\n    \"LastModified\": {},\n    \"ETag\": {},\n    \"Size\": {},\n    \"ChecksumCRC32\": {},\n    \"ChecksumCRC32C\": {},\n    \"ChecksumSHA1\": {},\n    \"ChecksumSHA256\": {}\n  },\n  \"description\": \"Container for elements related to a part.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-part-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Part
---
