---
description: Specifies the Amazon S3 object key name to filter on and whether to filter on the suffix or prefix of the key name.
layout: schema
name: FilterRule
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-filterrule-schema.json
slug: s3-filterrule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {},\n    \"Value\": {}\n  },\n  \"description\": \"Specifies the Amazon S3 object key name to filter on and whether to filter on the suffix or prefix of the key name.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-filterrule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: FilterRule
---
