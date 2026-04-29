---
description: A container for filter information for the selection of S3 objects encrypted with Amazon Web Services KMS.
layout: schema
name: SseKmsEncryptedObjects
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-ssekmsencryptedobjects-schema.json
slug: s3-ssekmsencryptedobjects
source_filename: s3-ssekmsencryptedobjects-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SseKmsEncryptedObjects\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"required\": [\n    \"Status\"\n  ],\n  \"description\": \"A container for filter information for the selection of S3 objects encrypted with Amazon Web Services KMS.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-ssekmsencryptedobjects-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SseKmsEncryptedObjects
---
