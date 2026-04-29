---
description: Describes the cross-origin access configuration for objects in an Amazon S3 bucket.
layout: schema
name: CORSConfiguration
properties_list:
- description: ''
  name: CORSRule
  type: array
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-cors-configuration-schema.json
slug: amazon-s3-rest-cors-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Describes the cross-origin access configuration for objects in an Amazon S3 bucket.\",\n  \"properties\": {\n    \"CORSRule\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-cors-configuration-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CORSConfiguration
---
