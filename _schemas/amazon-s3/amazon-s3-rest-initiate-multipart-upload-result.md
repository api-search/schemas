---
description: Container for response to initiate multipart upload.
layout: schema
name: InitiateMultipartUploadResult
properties_list:
- description: The name of the bucket to which the multipart upload was initiated.
  name: Bucket
  type: string
- description: Object key for which the multipart upload was initiated.
  name: Key
  type: string
- description: ID for the initiated multipart upload. This ID is used in all subsequent multipart upload operations.
  name: UploadId
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-initiate-multipart-upload-result-schema.json
slug: amazon-s3-rest-initiate-multipart-upload-result
source_filename: amazon-s3-rest-initiate-multipart-upload-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitiateMultipartUploadResult\",\n  \"type\": \"object\",\n  \"description\": \"Container for response to initiate multipart upload.\",\n  \"properties\": {\n    \"Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket to which the multipart upload was initiated.\"\n    },\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Object key for which the multipart upload was initiated.\"\n    },\n    \"UploadId\": {\n      \"type\": \"string\",\n      \"description\": \"ID for the initiated multipart upload. This ID is used in all subsequent multipart upload operations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-initiate-multipart-upload-result-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: InitiateMultipartUploadResult
---
