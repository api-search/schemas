---
description: The container for the completed multipart upload response.
layout: schema
name: CompleteMultipartUploadResult
properties_list:
- description: The URI that identifies the newly created object.
  name: Location
  type: string
- description: The name of the bucket that contains the newly created object.
  name: Bucket
  type: string
- description: The object key of the newly created object.
  name: Key
  type: string
- description: Entity tag that identifies the newly created object's data.
  name: ETag
  type: string
- description: ''
  name: ChecksumCRC32
  type: string
- description: ''
  name: ChecksumCRC32C
  type: string
- description: ''
  name: ChecksumSHA1
  type: string
- description: ''
  name: ChecksumSHA256
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-complete-multipart-upload-result-schema.json
slug: amazon-s3-rest-complete-multipart-upload-result
source_filename: amazon-s3-rest-complete-multipart-upload-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompleteMultipartUploadResult\",\n  \"type\": \"object\",\n  \"description\": \"The container for the completed multipart upload response.\",\n  \"properties\": {\n    \"Location\": {\n      \"type\": \"string\",\n      \"description\": \"The URI that identifies the newly created object.\"\n    },\n    \"Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket that contains the newly created object.\"\n    },\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The object key of the newly created object.\"\n    },\n    \"ETag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag that identifies the newly created object's data.\"\n    },\n    \"ChecksumCRC32\": {\n      \"type\": \"string\"\n    },\n    \"ChecksumCRC32C\": {\n      \"type\": \"string\"\n    },\n    \"ChecksumSHA1\": {\n      \"type\": \"string\"\n    },\n   \
  \ \"ChecksumSHA256\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-complete-multipart-upload-result-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CompleteMultipartUploadResult
---
