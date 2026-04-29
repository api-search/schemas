---
description: ''
layout: schema
name: DeleteMarkers
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-deletemarkers-schema.json
slug: s3-deletemarkers
source_filename: s3-deletemarkers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteMarkers\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Owner\": {},\n      \"Key\": {},\n      \"VersionId\": {},\n      \"IsLatest\": {},\n      \"LastModified\": {}\n    },\n    \"description\": \"Information about the delete marker.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-deletemarkers-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: DeleteMarkers
---
