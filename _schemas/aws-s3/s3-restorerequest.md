---
description: Container for restore job parameters.
layout: schema
name: RestoreRequest
properties_list:
- description: ''
  name: Days
  type: object
- description: ''
  name: GlacierJobParameters
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Tier
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SelectParameters
  type: object
- description: ''
  name: OutputLocation
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-restorerequest-schema.json
slug: s3-restorerequest
source_filename: s3-restorerequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RestoreRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Days\": {},\n    \"GlacierJobParameters\": {},\n    \"Type\": {},\n    \"Tier\": {},\n    \"Description\": {},\n    \"SelectParameters\": {},\n    \"OutputLocation\": {}\n  },\n  \"description\": \"Container for restore job parameters.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-restorerequest-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: RestoreRequest
---
