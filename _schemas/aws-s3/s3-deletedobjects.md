---
description: ''
layout: schema
name: DeletedObjects
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-deletedobjects-schema.json
slug: s3-deletedobjects
source_filename: s3-deletedobjects-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedObjects\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Key\": {},\n      \"VersionId\": {},\n      \"DeleteMarker\": {},\n      \"DeleteMarkerVersionId\": {}\n    },\n    \"description\": \"Information about the deleted object.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-deletedobjects-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: DeletedObjects
---
