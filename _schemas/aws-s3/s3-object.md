---
description: An object consists of data and its descriptive metadata.
layout: schema
name: Object
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: LastModified
  type: object
- description: ''
  name: ETag
  type: object
- description: ''
  name: ChecksumAlgorithm
  type: object
- description: ''
  name: Size
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: Owner
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-object-schema.json
slug: s3-object
source_filename: s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {},\n    \"LastModified\": {},\n    \"ETag\": {},\n    \"ChecksumAlgorithm\": {},\n    \"Size\": {},\n    \"StorageClass\": {},\n    \"Owner\": {}\n  },\n  \"description\": \"An object consists of data and its descriptive metadata.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-object-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Object
---
