---
description: Specifies JSON as request's output serialization format.
layout: schema
name: JSONOutput
properties_list:
- description: ''
  name: RecordDelimiter
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-jsonoutput-schema.json
slug: s3-jsonoutput
source_filename: s3-jsonoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JSONOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordDelimiter\": {}\n  },\n  \"description\": \"Specifies JSON as request's output serialization format.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-jsonoutput-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: JSONOutput
---
