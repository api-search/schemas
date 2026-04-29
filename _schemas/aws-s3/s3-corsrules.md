---
description: ''
layout: schema
name: CORSRules
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-corsrules-schema.json
slug: s3-corsrules
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSRules\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ID\": {},\n      \"AllowedHeaders\": {},\n      \"AllowedMethods\": {},\n      \"AllowedOrigins\": {},\n      \"ExposeHeaders\": {},\n      \"MaxAgeSeconds\": {}\n    },\n    \"required\": [\n      \"AllowedMethods\",\n      \"AllowedOrigins\"\n    ],\n    \"description\": \"Specifies a cross-origin access rule for an Amazon S3 bucket.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-corsrules-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CORSRules
---
