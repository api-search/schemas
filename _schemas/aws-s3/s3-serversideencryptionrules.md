---
description: ''
layout: schema
name: ServerSideEncryptionRules
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-serversideencryptionrules-schema.json
slug: s3-serversideencryptionrules
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerSideEncryptionRules\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ApplyServerSideEncryptionByDefault\": {},\n      \"BucketKeyEnabled\": {}\n    },\n    \"description\": \"Specifies the default server-side encryption configuration.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-serversideencryptionrules-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ServerSideEncryptionRules
---
