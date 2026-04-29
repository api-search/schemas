---
description: Describes the serialization format of the object.
layout: schema
name: InputSerialization
properties_list:
- description: ''
  name: CSV
  type: object
- description: ''
  name: CompressionType
  type: object
- description: ''
  name: JSON
  type: object
- description: ''
  name: Parquet
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inputserialization-schema.json
slug: s3-inputserialization
source_filename: s3-inputserialization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InputSerialization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CSV\": {},\n    \"CompressionType\": {},\n    \"JSON\": {},\n    \"Parquet\": {}\n  },\n  \"description\": \"Describes the serialization format of the object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inputserialization-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InputSerialization
---
