---
description: ''
layout: schema
name: ObjectStorageClass
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectstorageclass-schema.json
slug: s3-objectstorageclass
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectStorageClass\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"STANDARD\",\n    \"REDUCED_REDUNDANCY\",\n    \"GLACIER\",\n    \"STANDARD_IA\",\n    \"ONEZONE_IA\",\n    \"INTELLIGENT_TIERING\",\n    \"DEEP_ARCHIVE\",\n    \"OUTPOSTS\",\n    \"GLACIER_IR\",\n    \"SNOW\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectstorageclass-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectStorageClass
---
