---
description: A metadata key-value pair to store with an object.
layout: schema
name: MetadataEntry
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-metadataentry-schema.json
slug: s3-metadataentry
source_filename: s3-metadataentry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetadataEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {},\n    \"Value\": {}\n  },\n  \"description\": \"A metadata key-value pair to store with an object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-metadataentry-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: MetadataEntry
---
