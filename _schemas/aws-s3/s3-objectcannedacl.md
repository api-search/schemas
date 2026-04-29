---
description: ''
layout: schema
name: ObjectCannedACL
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectcannedacl-schema.json
slug: s3-objectcannedacl
source_filename: s3-objectcannedacl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectCannedACL\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"private\",\n    \"public-read\",\n    \"public-read-write\",\n    \"authenticated-read\",\n    \"aws-exec-read\",\n    \"bucket-owner-read\",\n    \"bucket-owner-full-control\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectcannedacl-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectCannedACL
---
