---
description: Describes how results of the Select job are serialized.
layout: schema
name: OutputSerialization
properties_list:
- description: ''
  name: CSV
  type: object
- description: ''
  name: JSON
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-outputserialization-schema.json
slug: s3-outputserialization
source_filename: s3-outputserialization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutputSerialization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CSV\": {},\n    \"JSON\": {}\n  },\n  \"description\": \"Describes how results of the Select job are serialized.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-outputserialization-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: OutputSerialization
---
