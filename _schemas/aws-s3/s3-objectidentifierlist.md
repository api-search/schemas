---
description: ''
layout: schema
name: ObjectIdentifierList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectidentifierlist-schema.json
slug: s3-objectidentifierlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectIdentifierList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Key\": {},\n      \"VersionId\": {}\n    },\n    \"required\": [\n      \"Key\"\n    ],\n    \"description\": \"Object Identifier is unique value to identify objects.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectidentifierlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectIdentifierList
---
