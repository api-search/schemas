---
description: Container for the <code>MultipartUpload</code> for the Amazon S3 object.
layout: schema
name: MultipartUpload
properties_list:
- description: ''
  name: UploadId
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: Initiated
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: Initiator
  type: object
- description: ''
  name: ChecksumAlgorithm
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-multipartupload-schema.json
slug: s3-multipartupload
source_filename: s3-multipartupload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MultipartUpload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UploadId\": {},\n    \"Key\": {},\n    \"Initiated\": {},\n    \"StorageClass\": {},\n    \"Owner\": {},\n    \"Initiator\": {},\n    \"ChecksumAlgorithm\": {}\n  },\n  \"description\": \"Container for the <code>MultipartUpload</code> for the Amazon S3 object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-multipartupload-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: MultipartUpload
---
