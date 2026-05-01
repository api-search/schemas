---
description: ''
layout: schema
name: Permission
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-permission-schema.json
slug: s3-permission
source_filename: s3-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Permission\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FULL_CONTROL\",\n    \"WRITE\",\n    \"WRITE_ACP\",\n    \"READ\",\n    \"READ_ACP\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-permission-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Permission
---
