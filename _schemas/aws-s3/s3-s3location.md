---
description: Describes an Amazon S3 location that will receive the results of the restore request.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: Prefix
  type: object
- description: Contains the type of server-side encryption used.
  name: Encryption
  type: object
- description: ''
  name: CannedACL
  type: object
- description: ''
  name: AccessControlList
  type: object
- description: ''
  name: Tagging
  type: object
- description: ''
  name: UserMetadata
  type: object
- description: ''
  name: StorageClass
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-s3location-schema.json
slug: s3-s3location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"S3Location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {},\n    \"Prefix\": {},\n    \"Encryption\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"EncryptionType\": {},\n        \"KMSKeyId\": {},\n        \"KMSContext\": {}\n      },\n      \"required\": [\n        \"EncryptionType\"\n      ],\n      \"description\": \"Contains the type of server-side encryption used.\"\n    },\n    \"CannedACL\": {},\n    \"AccessControlList\": {},\n    \"Tagging\": {},\n    \"UserMetadata\": {},\n    \"StorageClass\": {}\n  },\n  \"required\": [\n    \"BucketName\",\n    \"Prefix\"\n  ],\n  \"description\": \"Describes an Amazon S3 location that will receive the results of the restore request.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-s3location-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: S3Location
---
