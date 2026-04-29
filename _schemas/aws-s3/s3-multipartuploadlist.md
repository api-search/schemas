---
description: ''
layout: schema
name: MultipartUploadList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-multipartuploadlist-schema.json
slug: s3-multipartuploadlist
source_filename: s3-multipartuploadlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MultipartUploadList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"UploadId\": {},\n      \"Key\": {},\n      \"Initiated\": {},\n      \"StorageClass\": {},\n      \"Owner\": {},\n      \"Initiator\": {},\n      \"ChecksumAlgorithm\": {}\n    },\n    \"description\": \"Container for the <code>MultipartUpload</code> for the Amazon S3 object.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-multipartuploadlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: MultipartUploadList
---
