---
description: A legal hold configuration for an object.
layout: schema
name: ObjectLockLegalHold
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectlocklegalhold-schema.json
slug: s3-objectlocklegalhold
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectLockLegalHold\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"description\": \"A legal hold configuration for an object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectlocklegalhold-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectLockLegalHold
---
