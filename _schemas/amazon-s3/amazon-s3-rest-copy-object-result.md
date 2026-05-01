---
description: Container for all response elements.
layout: schema
name: CopyObjectResult
properties_list:
- description: Returns the ETag of the new object.
  name: ETag
  type: string
- description: Creation date of the object.
  name: LastModified
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
schema_file: json-schema/amazon-s3-rest-copy-object-result-schema.json
slug: amazon-s3-rest-copy-object-result
source_filename: amazon-s3-rest-copy-object-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopyObjectResult\",\n  \"type\": \"object\",\n  \"description\": \"Container for all response elements.\",\n  \"properties\": {\n    \"ETag\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the ETag of the new object.\"\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"Creation date of the object.\"\n    },\n    \"ChecksumCRC32\": {\n      \"type\": \"string\"\n    },\n    \"ChecksumCRC32C\": {\n      \"type\": \"string\"\n    },\n    \"ChecksumSHA1\": {\n      \"type\": \"string\"\n    },\n    \"ChecksumSHA256\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-copy-object-result-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CopyObjectResult
---
