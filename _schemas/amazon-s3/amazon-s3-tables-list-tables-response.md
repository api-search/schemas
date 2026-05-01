---
description: ''
layout: schema
name: ListTablesResponse
properties_list:
- description: ''
  name: tables
  type: array
- description: ''
  name: continuationToken
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-list-tables-response-schema.json
slug: amazon-s3-tables-list-tables-response
source_filename: amazon-s3-tables-list-tables-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTablesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tables\": {\n      \"type\": \"array\"\n    },\n    \"continuationToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-list-tables-response-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: ListTablesResponse
---
