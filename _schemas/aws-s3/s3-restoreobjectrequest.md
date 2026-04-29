---
description: ''
layout: schema
name: RestoreObjectRequest
properties_list:
- description: Container for restore job parameters.
  name: RestoreRequest
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-restoreobjectrequest-schema.json
slug: s3-restoreobjectrequest
source_filename: s3-restoreobjectrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RestoreObjectRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RestoreRequest\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Days\": {},\n        \"GlacierJobParameters\": {},\n        \"Type\": {},\n        \"Tier\": {},\n        \"Description\": {},\n        \"SelectParameters\": {},\n        \"OutputLocation\": {}\n      },\n      \"description\": \"Container for restore job parameters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-restoreobjectrequest-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: RestoreObjectRequest
---
