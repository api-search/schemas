---
description: Specifies encryption-related information for an Amazon S3 bucket that is a destination for replicated objects.
layout: schema
name: EncryptionConfiguration
properties_list:
- description: ''
  name: ReplicaKmsKeyID
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-encryptionconfiguration-schema.json
slug: s3-encryptionconfiguration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EncryptionConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicaKmsKeyID\": {}\n  },\n  \"description\": \"Specifies encryption-related information for an Amazon S3 bucket that is a destination for replicated objects.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-encryptionconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: EncryptionConfiguration
---
