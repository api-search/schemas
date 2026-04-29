---
description: The container element for a bucket's policy status.
layout: schema
name: PolicyStatus
properties_list:
- description: ''
  name: IsPublic
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-policystatus-schema.json
slug: s3-policystatus
source_filename: s3-policystatus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsPublic\": {}\n  },\n  \"description\": \"The container element for a bucket's policy status.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-policystatus-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: PolicyStatus
---
