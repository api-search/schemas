---
description: Container for S3 Glacier job parameters.
layout: schema
name: GlacierJobParameters
properties_list:
- description: ''
  name: Tier
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-glacierjobparameters-schema.json
slug: s3-glacierjobparameters
source_filename: s3-glacierjobparameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlacierJobParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tier\": {}\n  },\n  \"required\": [\n    \"Tier\"\n  ],\n  \"description\": \"Container for S3 Glacier job parameters.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-glacierjobparameters-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: GlacierJobParameters
---
