---
description: A container for object key name prefix and suffix filtering rules.
layout: schema
name: S3KeyFilter
properties_list:
- description: ''
  name: FilterRules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-s3keyfilter-schema.json
slug: s3-s3keyfilter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"S3KeyFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilterRules\": {}\n  },\n  \"description\": \"A container for object key name prefix and suffix filtering rules.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-s3keyfilter-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: S3KeyFilter
---
