---
description: Contains the type of server-side encryption used.
layout: schema
name: Encryption
properties_list:
- description: ''
  name: EncryptionType
  type: object
- description: ''
  name: KMSKeyId
  type: object
- description: ''
  name: KMSContext
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-encryption-schema.json
slug: s3-encryption
source_filename: s3-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Encryption\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncryptionType\": {},\n    \"KMSKeyId\": {},\n    \"KMSContext\": {}\n  },\n  \"required\": [\n    \"EncryptionType\"\n  ],\n  \"description\": \"Contains the type of server-side encryption used.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-encryption-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Encryption
---
