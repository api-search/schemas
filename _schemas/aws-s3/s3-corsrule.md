---
description: Specifies a cross-origin access rule for an Amazon S3 bucket.
layout: schema
name: CORSRule
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: AllowedHeaders
  type: object
- description: ''
  name: AllowedMethods
  type: object
- description: ''
  name: AllowedOrigins
  type: object
- description: ''
  name: ExposeHeaders
  type: object
- description: ''
  name: MaxAgeSeconds
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-corsrule-schema.json
slug: s3-corsrule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {},\n    \"AllowedHeaders\": {},\n    \"AllowedMethods\": {},\n    \"AllowedOrigins\": {},\n    \"ExposeHeaders\": {},\n    \"MaxAgeSeconds\": {}\n  },\n  \"required\": [\n    \"AllowedMethods\",\n    \"AllowedOrigins\"\n  ],\n  \"description\": \"Specifies a cross-origin access rule for an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-corsrule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CORSRule
---
