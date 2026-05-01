---
description: Container for grant information.
layout: schema
name: Grant
properties_list:
- description: ''
  name: Grantee
  type: object
- description: ''
  name: Permission
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-grant-schema.json
slug: s3-grant
source_filename: s3-grant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Grant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Grantee\": {},\n    \"Permission\": {}\n  },\n  \"description\": \"Container for grant information.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-grant-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Grant
---
