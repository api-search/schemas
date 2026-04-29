---
description: Object Identifier is unique value to identify objects.
layout: schema
name: ObjectIdentifier
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectidentifier-schema.json
slug: s3-objectidentifier
source_filename: s3-objectidentifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectIdentifier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {},\n    \"VersionId\": {}\n  },\n  \"required\": [\n    \"Key\"\n  ],\n  \"description\": \"Object Identifier is unique value to identify objects.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectidentifier-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectIdentifier
---
