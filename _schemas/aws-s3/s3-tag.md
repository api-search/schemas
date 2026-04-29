---
description: A container of a key value name pair.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-tag-schema.json
slug: s3-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {},\n    \"Value\": {}\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ],\n  \"description\": \"A container of a key value name pair.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-tag-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Tag
---
