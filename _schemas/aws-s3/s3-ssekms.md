---
description: Specifies the use of SSE-KMS to encrypt delivered inventory reports.
layout: schema
name: SSEKMS
properties_list:
- description: ''
  name: KeyId
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-ssekms-schema.json
slug: s3-ssekms
source_filename: s3-ssekms-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SSEKMS\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyId\": {}\n  },\n  \"required\": [\n    \"KeyId\"\n  ],\n  \"description\": \"Specifies the use of SSE-KMS to encrypt delivered inventory reports.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-ssekms-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SSEKMS
---
