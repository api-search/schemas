---
description: ''
layout: schema
name: ObjectAttributesList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectattributeslist-schema.json
slug: s3-objectattributeslist
source_filename: s3-objectattributeslist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectAttributesList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"ETag\",\n      \"Checksum\",\n      \"ObjectParts\",\n      \"StorageClass\",\n      \"ObjectSize\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectattributeslist-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: ObjectAttributesList
---
