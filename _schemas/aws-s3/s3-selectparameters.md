---
description: Describes the parameters for Select job types.
layout: schema
name: SelectParameters
properties_list:
- description: ''
  name: InputSerialization
  type: object
- description: ''
  name: ExpressionType
  type: object
- description: ''
  name: Expression
  type: object
- description: ''
  name: OutputSerialization
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-selectparameters-schema.json
slug: s3-selectparameters
source_filename: s3-selectparameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelectParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputSerialization\": {},\n    \"ExpressionType\": {},\n    \"Expression\": {},\n    \"OutputSerialization\": {}\n  },\n  \"required\": [\n    \"InputSerialization\",\n    \"ExpressionType\",\n    \"Expression\",\n    \"OutputSerialization\"\n  ],\n  \"description\": \"Describes the parameters for Select job types.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-selectparameters-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: SelectParameters
---
