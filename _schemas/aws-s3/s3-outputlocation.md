---
description: Describes the location where the restore job's output is stored.
layout: schema
name: OutputLocation
properties_list:
- description: ''
  name: S3
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-outputlocation-schema.json
slug: s3-outputlocation
source_filename: s3-outputlocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutputLocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3\": {}\n  },\n  \"description\": \"Describes the location where the restore job's output is stored.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-outputlocation-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: OutputLocation
---
