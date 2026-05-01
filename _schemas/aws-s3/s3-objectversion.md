---
description: The version of an object.
layout: schema
name: ObjectVersion
properties_list:
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
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
- description: ''
  name: IsLatest
  type: object
- description: ''
  name: LastModified
  type: object
- description: ''
  name: Owner
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectversion-schema.json
slug: s3-objectversion
source_filename: s3-objectversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectVersion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ETag\": {},\n    \"ChecksumAlgorithm\": {},\n    \"Size\": {},\n    \"StorageClass\": {},\n    \"Key\": {},\n    \"VersionId\": {},\n    \"IsLatest\": {},\n    \"LastModified\": {},\n    \"Owner\": {}\n  },\n  \"description\": \"The version of an object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectversion-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: ObjectVersion
---
